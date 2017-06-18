# vue-drag-tree

> It's a tree components(Vue2.x) that allow you to drag and drop the node to exchange their data .

**Feature**

- Double click on an item to turn it into a folder
- Drag and drop the tree node, even between two different levels

**[中文](README_ZH.md)**

### Demo

---

![demo](static/vue-drag-tree.gif)

### Getting Start

---

**Install**

`npm install vue-drag-tree --save`

**Usage**

main.js

```vue
import Vue from 'vue'
import VueDragTree from 'vue-drag-tree'

Vue.component('vue-drag-tree', VueDragTree)
```

test.vue

```vue
<template>
	<vue-darg-tree :model='data'></vue-drag-tree>
</template>
<script>
export default{
  data(){
    return{
      data:{
        name: 'Root',
        id: 0,
        children: [
          {
            name: 'Node 1-1',
            id: 1
            children: [
              {
                name: 'Node 2-1',
                id: 2
              }
            ]
          },
          {
            name: 'Node 1-2',
            id: 3
          }
        ]
      }
    }
  }
}
<script>
```

**License**

---

[MIT](LICENSE)