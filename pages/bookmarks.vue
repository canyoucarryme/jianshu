<template>
    <div style="height:100%">
        <my-header></my-header>
        <div class="container bookmarks" id="js-page-top">
            <div class="row">
                <div class="col-xs-18 col-xs-offset-3 main">
                    <img class="tag-banner" src="~/assets/img/collect-note.png" alt="Collect note">
                    <!-- 文章列表模块 -->
                    <ul class="note-list">

                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
     import myHeader from "~/components/myHeader"
    export default {
    components: {
        myHeader,

    },
    data() {
        return {
        };
    } 
};   
</script>

<style scoped>
    .bookmarks .row{
        padding-top: 30px;
    }
    .tag-banner{
        margin-bottom: 30px;
        width: 100%;
        min-height: 100px;
        background-color: hsla(0,0%,71%,.2);
        border-radius: 6px;
    }
</style>
