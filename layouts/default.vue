<template>
  <v-app dark>
    <v-navigation-drawer
      :mini-variant="miniVariant"
      :clipped="clipped"
      v-model="drawer"
      fixed
      app
    >
      <v-list>
        <v-list-tile
          :to="item.to"
          :key="i"
          v-for="(item, i) in items"
          exact
        >
          <v-list-tile-action>
            <v-icon v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar 
          fixed 
          app 
          :clipped-left="clipped">
      <v-toolbar-side-icon @click.stop ="drawer = !drawer" ></v-toolbar-side-icon>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    
    <v-footer :fixed="fixed" app>
      <span>&copy; 2018</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data() {
      return {
        clipped: false,
        drawer: false,
        fixed: false,
        items: [
          { icon: 'home', title: 'На главную', to: '/' },
          { icon: 'person', title: 'Биография', to: '/bio' },
          { icon: 'folder', title: 'Личное дело', to: '/resume' },
          { icon: 'people', title: 'Друзья, Однокашники', to: '/friends' },
          { icon: 'beenhere', title: 'Воспоминания', to: '/memory' },
          { icon: 'tv', title: 'Сми о Нуриеве', to: '/media' },
          { icon: 'photo_camera', title: 'Кино фото документы', to: '/photo' }
        ],
        miniVariant: false,
        title: 'Борис Исаевич Нуриев'
      }
    }
  }
</script>
