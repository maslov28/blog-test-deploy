<template>
    <div class="slider">
        <div class="slider__wrapper">
            <div 
                class="slider__items" 
                :style="{'margin-left': '-' + (100 * currentSlide) + '%'}"
            >
                <slot></slot>
            </div>
        </div>
        <div class="slider__prevnext-btn" v-if="prevNextBtn">
            <div class="slider__prev-btn-wrapper">
                <span class="slider__prev-btn" @click="previousSlide"></span>
            </div>
            <div class="slider__next-btn-wrapper">
                <span class="slider__next-btn" @click="nextSlide"></span>
            </div>
        </div>
        <div class="slider__dot-buttons" v-if="dotBtn">
            <span 
                class="slider__dot-btn" 
                :class="{'slider__dot-btn--active': currentSlide === idx }"
                v-for="(button, idx) of countSlide" 
                :key="button" 
                @click="currentSlide = idx"
            ></span>
        </div>
    </div>
</template>

<script>
import { ref } from 'vue'
export default {
    props: {
        dotBtn: {
            type: Boolean,
            default: false
        },
        prevNextBtn: {
            type: Boolean,
            default: false
        },
        countSlide: {
            type: Number,
            default: 1
        }
    },
    setup(props) {
        const currentSlide = ref(0)

        const nextSlide = () => {
            if (currentSlide.value < props.countSlide - 1) {
                currentSlide.value++
            }
        }
        const previousSlide = () => {
            if (currentSlide.value !== 0) {
                currentSlide.value--
            }
        }

        return {
            currentSlide,
            nextSlide,
            previousSlide
        }
    }
}
</script>

<style lang="scss">
.slider {
    &__wrapper {
        overflow: hidden;
    }
    &__items {
        display: flex;
        transition: all ease .5s;
    }
    &__dot-buttons {
        text-align: center;
        padding-top: 26px;
    }
    &__prevnext-btn {
        display: flex;
    }
    &__prev-btn, .slider__next-btn {
        display: inline-block;
        cursor: pointer;
        width: 40px;
        height: 40px;
        background-color: $main-color;
        border-radius: 50%;
        transition: all ease .2s;
    }
    &__prev-btn:hover, .slider__next-btn:hover {
        opacity: .5;
    }
    &__prev-btn {
        position: relative;
    }
    &__prev-btn::after {
        content: '';
        position: absolute;
        width: 12px;
        height: 18px;
        top: 11px;
        left: 13px;
        background: url('@/assets/img/arrow-left.svg') no-repeat center center;
    }
    &__next-btn {
        position: relative;
    }
    &__next-btn::after {
        content: '';
        position: absolute;
        width: 12px;
        height: 18px;
        top: 11px;
        right: 13px;
        background: url('@/assets/img/arrow-right.svg') no-repeat center center;
    }
    &__dot-btn {
        display: inline-block;
        width: 8px;
        height: 8px;
        background-color: $slider-no-active;
        border-radius: 50%;
        cursor: pointer;
    }
    &__dot-btn:not(:last-child) {
        margin-right: 20px;
    }
    &__dot-btn--active {
        background-color: $slider-active;
    }
}
</style>