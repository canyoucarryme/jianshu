<template>
    <div style="height:100%">
        <my-header></my-header>
        <div class="container setting">
            <div class="row">
                <div class="aside">
                    <ul>
                        <li>
                            <nuxt-link to="/settings/basic">
                                <div class="setting-icon">
                                    <i class="fa fa-list-ul"></i>
                                </div>
                                <span>基础设置</span>
                            </nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/settings/basic">
                                <div class="setting-icon">
                                    <i class="fa fa-user-plus"></i>
                                </div>
                                <span>个人资料</span>
                            </nuxt-link>
                        </li>
                          <li>
                            <nuxt-link to="/settings/basic">
                                <div class="setting-icon">
                                    <i class="fa fa-address-book"></i>
                                </div>
                                <span>微博认证</span>
                            </nuxt-link>
                        </li>
                          <li>
                            <nuxt-link to="/settings/basic">
                                <div class="setting-icon">
                                    <i class="fa fa-address-book"></i>
                                </div>
                                <span>基础设置</span>
                            </nuxt-link>
                        </li>
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
    
</style>
