<template>
    <div>
        <div class="row">
            <div class="col-12">

                <b-navbar toggleable="lg" type="light" variant="">
                    <b-navbar-brand href="#">NavBar</b-navbar-brand>

                    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

                    <b-collapse id="nav-collapse" is-nav>

                        <b-navbar-nav>
                            <b-nav-item href="#">Link</b-nav-item>
                            <b-nav-item href="#" disabled>Disabled</b-nav-item>
                        </b-navbar-nav>

                        <!-- Right aligned nav items -->
                        <b-navbar-nav class="ml-auto">

                            <b-nav-item-dropdown text="Lang" right>
                                <b-dropdown-item href="#">EN</b-dropdown-item>
                                <b-dropdown-item href="#">ES</b-dropdown-item>
                                <b-dropdown-item href="#">RU</b-dropdown-item>
                                <b-dropdown-item href="#">FA</b-dropdown-item>
                            </b-nav-item-dropdown>

                            <b-nav-item-dropdown right>
                                <!-- Using 'button-content' slot -->
                                <template #button-content>
                                    <em>User</em>
                                </template>
                                <b-dropdown-item href="#">Profile</b-dropdown-item>
                                <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                            </b-nav-item-dropdown>

                        </b-navbar-nav>

                    </b-collapse>

                </b-navbar>

            </div>
        </div>

        <div class="row justify-content-center">
            <div class="col-lg-6 searchbox-container">
                
                <h1 class="omi-title">OMI Search</h1>
                <SearchBox />

            </div>
        </div>

    </div>
</template>

<script>
import SearchBox from './SearchBox.vue'

export default {
  components: { SearchBox },
    name: 'Search'
}
</script>

<style>
    .searchbox-container {
        padding-top: 20vh;
    }
    .omi-title {
        font-family: 'Potta One', cursive;
        font-size: 100px;
        margin: 20px 0;
        text-align: center;
    }
</style>