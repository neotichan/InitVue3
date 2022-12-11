<template>
    <div>
        <h2>Router</h2>
        <router-link to="/top">/topのComponent内容を表示</router-link>
        <router-link to="/second">/secondのComponent内容を表示</router-link>
       <router-view></router-view>
    </div>
</template>
<script>

export default {
    name:"RouterComponent",
    routes:[
        {path:'/top',
            component:{
            template:'<div>トップページ</div>'
            }
        },
        {path:'/second',
            component:{
            template:'<div>Routerで切り替えたページです</div>'
            }
        }
    ]
}
</script>