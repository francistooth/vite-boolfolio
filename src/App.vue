<script>
import { RouterLink } from 'vue-router';
</script>

<template>
    <div>
        <nav>
            <ul>
                <li> 
                    <router-link :to="{name: 'home'}">  
                        Home Page
                    </router-link> 
                </li>

                <li> 
                    <router-link :to="{name: 'works'}">  
                        Progetti
                    </router-link> 
                </li>
            </ul>
        </nav>
        <router-view>

        </router-view>
    </div>
</template>

<style lang="scss">

</style>