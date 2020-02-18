<template lang="pug">
    main.container

        section.content-left

            div.up

                div.up-content.left
                    div.title 
                        <svg xmlns="http://www.w3.org/2000/svg" width="21" height="21" viewBox="0 0 21 21"><defs><style>.a{fill:#707070;}</style></defs><path class="a" d="M0,16.624v1.751C0,19.823,3.527,21,7.875,21s7.875-1.177,7.875-2.625V16.624c-1.694,1.194-4.791,1.751-7.875,1.751S1.694,17.817,0,16.624ZM13.125,5.25C17.473,5.25,21,4.073,21,2.625S17.473,0,13.125,0,5.25,1.177,5.25,2.625,8.777,5.25,13.125,5.25ZM0,12.321v2.116c0,1.448,3.527,2.625,7.875,2.625s7.875-1.177,7.875-2.625V12.321c-1.694,1.395-4.795,2.116-7.875,2.116S1.694,13.716,0,12.321Zm17.063.451C19.413,12.317,21,11.472,21,10.5V8.749a10.072,10.072,0,0,1-3.937,1.415ZM7.875,6.563C3.527,6.563,0,8.031,0,9.844s3.527,3.281,7.875,3.281,7.875-1.468,7.875-3.281S12.223,6.563,7.875,6.563ZM16.87,8.872C19.331,8.429,21,7.559,21,6.563V4.811c-1.456,1.029-3.958,1.583-6.591,1.714A4.593,4.593,0,0,1,16.87,8.872Z"/></svg>
                        span Seu investimento
                    div.middle-left
                        p Saldo:
                        span R$
                            font 20,
                            |00
                        p.margin Complete as fases e recebe cashback para investir.

                div.up-content.right
                    div.title 
                        <svg xmlns="http://www.w3.org/2000/svg" width="26.25" height="21" viewBox="0 0 26.25 21"><defs><style>.a{fill:#707070;}</style></defs><path class="a" d="M21.656,18.375H4.594a.658.658,0,0,0-.656.656v1.313A.658.658,0,0,0,4.594,21H21.656a.658.658,0,0,0,.656-.656V19.031A.658.658,0,0,0,21.656,18.375ZM24.281,5.25a1.969,1.969,0,0,0-1.969,1.969,1.929,1.929,0,0,0,.18.812l-2.97,1.78a1.311,1.311,0,0,1-1.813-.476L14.368,3.486a1.969,1.969,0,1,0-2.486,0L8.539,9.335a1.312,1.312,0,0,1-1.813.476L3.761,8.031A1.968,1.968,0,1,0,1.969,9.188a2.01,2.01,0,0,0,.316-.033L5.25,17.063H21l2.965-7.908a2.011,2.011,0,0,0,.316.033,1.969,1.969,0,0,0,0-3.937Z"/></svg>
                        span Seu nível

                    div.middle-right
                        span Iniciante
                        p Complete as fases e suba de nível para
                            | desbloquear novas funções.

            div.down

                div.down-learn1

                div.down-learn2

        section.menu-right
</template>

<script>
export default {
    
}
</script>

<style lang="sass" scoped>

    .container
        width: 100%
        height: 100%
        display: flex
        position: relative
        background-color: #F2F2F2

        .content-left 
            padding: 40px 60px
            width: calc(100% - 120px)
            box-sizing: border-box
            display: flex
            justify-content: space-between
            flex-direction: column

            .up
                height: 200px
                display: flex
                justify-content: center

                .up-content
                    height: 170px
                    width: 440px
                    background-color: white
                    box-shadow: 1px 0px 8px rgba(0,0,0,0.06)
                    padding: 30px
                    box-sizing: border-box

                    .title
                        display: flex
                        align-items: center
                        height: fit-content
                    
                        span
                            margin-left: 10px
                            color: #707070
                            font-size: 18px
                            font-weight: bold

                    .middle-left
                        padding-top: 18px
                        p 
                            font-size: 14px
                            color: #BBBBBB

                        span
                            font-size: 32px
                            color: #01C676

                        font 
                            margin-left: 8px
                            font-weight: bold

                        .margin 
                            margin-top: 5px

                    .middle-right
                        padding-top: 15px
                        span 
                            font-size: 32px
                            color: #01C676
                        
                        p 
                            font-size: 14px
                            color: #BBBBBB
                            margin-top: 10px

                .left
                    margin-right: 40px
                    border-radius: 0px 10px
                .right
                    border-radius: 10px 0px 


            .down 
                height: 100%
                display: flex
                justify-content: center
                padding-top: 30px

                .down-learn1
                    height: 100%
                    width: 440px
                    background-color: white
                    border-radius: 10px 0px 
                    margin-right: 40px

                .down-learn2
                    height: 100%
                    width: 440px
                    background-color: white
                    border-radius: 0px 10px 

        .menu-right
            position: fixed
            height: 100%
            background-color: #01C676
            width: 120px
            right: 0
            top: 0
            box-shadow: -1px 0 8px rgba(0,0,0, 0.08)

        
        

</style>