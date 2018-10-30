<template>
    <div class="container">
        <div class="row">
            <p v-change-background-color-green> Test </p>
            <button> change text color </button>
            <button> change background color </button>
            <button> change text font </button>
        </div>
    </div>
</template>

<script>
    export default {
        directives: {
            'change-color-green': {
                bind(el, binding, vnode){
                    el.style.color = 'green';
                }    
            },
            
            'change-color-black': {
                bind(el, binding, vnode){
                    el.style.color = 'black';
                }    
            },
            
            'change-color-red': {
                bind(el, binding, vnode){
                    el.style.color = 'red';
                }    
            },
            
            'change-background-color-red': {
                bind(el, binding, vnode){
                    el.style.backgroundColor = 'red';
                }
            },
            
            'change-background-color-green': {
                bind(el, binding, vnode){
                    el.style.backgroundColor = 'green';
                }
            },
            
            'change-font-arizonia': {
                bind(el, binding, vnode){
                     el.style.fontFamily = 'Arizonia'; cursive;
                }    
            },

            'change-font': {
                bind(el, binding, vnode){
                    el.style.fontFamily = '';
                }    
            },
            
            'change-font': {
                bind(el, binding, vnode){
                    el.style.fontFamily = '';
                }    
            },
            
            // 'local-highlight': {
            //     bind(el, binding, vnode) {
            //         var delay = 0;
            //         if (binding.modifiers['delayed']) {
            //             delay = 3000;
            //         }
            //         if (binding.modifiers['blink']) {
            //             let mainColor = binding.value.mainColor;
            //             let secondColor = binding.value.secondColor;
            //             let currentColor = mainColor;
            //             setTimeout(() => {
            //                 setInterval(() => {
            //                     currentColor == secondColor ? currentColor = mainColor : currentColor = secondColor;
            //                     if (binding.arg == 'background') {
            //                         el.style.backgroundColor = currentColor;
            //                     } else {
            //                         el.style.color = currentColor;
            //                     }
            //                 }, binding.value.delay);
            //             }, delay);
            //         } else {
            //             setTimeout(() => {
            //                 if (binding.arg == 'background') {
            //                     el.style.backgroundColor = binding.value.mainColor;
            //                 } else {
            //                     el.style.color = binding.value.mainColor;
            //                 }
            //             }, delay);
            //         }
            //     }
            // }
        }
    }
</script>

<style>
</style>
