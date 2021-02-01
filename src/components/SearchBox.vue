<template>
    <form action="" method="get">
        <div class="input-group">
            <b-form-input name="searchbox" placeholder="Search the web"></b-form-input>
            <div class="input-group-append">
                <b-button variant="secondary">
                    <b-icon-search></b-icon-search>
                </b-button>
            </div>
        </div>
    </form>
</template>

<script>
export default {
    name: 'SearchBox'
}
</script>

