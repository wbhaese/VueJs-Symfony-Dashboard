<template>
    <div class="main">
        <div class="sidebar">
            <SideBarComponent />
        </div>

        <div class="content-right">
            <div class="navbar">
                <NavBarComponent />
            </div>

            <div class="pages">
                <slot name="slot-pages"></slot>
            </div>
        </div>
    </div>    
</template>

<script>
    import SideBarComponent from './components/SideBarComponent';
    import NavBarComponent from './components/NavBarComponent';

    export default {
        name: 'DashBoardComponent',
        components: {
            SideBarComponent,
            NavBarComponent,
        },
    }
</script>

<style lang="scss" src="./style.scss" scoped />
