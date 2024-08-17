<template>
  <div class="dropdown" @click="toggleDropdown">
    <a class="header__nav-link" href="#">{{ title }}
      <svg :class="{ 'rotated': isOpen }" width="11" height="7" viewBox="0 0 11 7" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M10.1845 1.55953L5.80953 5.93453C5.7689 5.97521 5.72065 6.00748 5.66754 6.02949C5.61442 6.05151 5.55749 6.06284 5.5 6.06284C5.4425 6.06284 5.38557 6.05151 5.33246 6.02949C5.27935 6.00748 5.2311 5.97521 5.19047 5.93453L0.815468 1.55953C0.733375 1.47744 0.687256 1.3661 0.687256 1.25C0.687256 1.1339 0.733375 1.02256 0.815468 0.940468C0.897561 0.858375 1.0089 0.812256 1.125 0.812256C1.2411 0.812256 1.35244 0.858375 1.43453 0.940468L5.5 5.00648L9.56547 0.940468C9.60612 0.899819 9.65437 0.867576 9.70748 0.845577C9.76059 0.823578 9.81751 0.812256 9.875 0.812256C9.93248 0.812256 9.98941 0.823578 10.0425 0.845577C10.0956 0.867576 10.1439 0.899819 10.1845 0.940468C10.2252 0.981116 10.2574 1.02937 10.2794 1.08248C10.3014 1.13559 10.3127 1.19251 10.3127 1.25C10.3127 1.30748 10.3014 1.36441 10.2794 1.41752C10.2574 1.47063 10.2252 1.51888 10.1845 1.55953Z" fill="#FFFFFF99"/>
      </svg>
    </a>
    <transition name="fade" appear>
      <ul class="dropdown__submenu" v-if="isOpen">
        <li v-for="(item, i) in items" :key="i"  class="dropdown__submenu-item" >
          <a class="dropdown__nav-link" :href="item.link">{{ item.title }}</a>
        </li>
      </ul>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'DropdownComponent',
  props: ['title', 'items'],
  data() {
    return {
      isOpen: false,
    }
  },
  methods: {
    toggleDropdown() {
      this.isOpen = !this.isOpen;
    }
  }
}
</script>

<style>
svg {
  margin-left: 3px;
  transition: transform 0.3s;
}

.rotated {
  transform: rotate(180deg);
}

.dropdown {
  width: max-content;
  position: relative;
  padding: 5px 13px;
  border-radius: 5px;
}

.dropdown__submenu {
  display: flex;
  width: 100%;
  flex-direction: column;
  position: absolute;
  top: calc(100% + 10px);
  left: 0;
  background-color: #222;
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 5px;
}

.dropdown__submenu-item {
  padding: 5px 13px;
}

.dropdown__submenu-item:hover {
  background-color: #333;
}
</style>
