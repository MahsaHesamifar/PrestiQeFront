<template>
  <v-container>
    <v-tabs
      v-model="tab"
      class="rounded-lg"
      align-tabs="center"
      bg-color="#21263d"
      fixed-tabs
      grow
    >
      <v-tab value="trophy"> کمد افتخارات</v-tab>
      <v-tab value="SocialActivity">فعالیت های اجتماعی</v-tab>
      <v-tab v-if="isPlayerView" value="Events">ایونت های پیشرو</v-tab>
    </v-tabs>

    <v-tabs-window v-model="tab">
      <v-tabs-window-item value="trophy">
        <TrophyTable />
      </v-tabs-window-item>

      <v-tabs-window-item value="SocialActivity">
        <socialActivity />
      </v-tabs-window-item>

      <v-tabs-window-item value="Events">
        <eventTable />
      </v-tabs-window-item>
    </v-tabs-window>
  </v-container>
</template>

<script>
import TrophyTable from "./TrophyTable.vue";
import eventTable from "./events.vue";
import socialActivity from "./socialActivity.vue";
export default {
  components: {
    TrophyTable,
    socialActivity,
    eventTable,
  },
  props: {
    isPlayerView: {
      type: Boolean,
      default: true,
    },
  },
  data() {
    return {
      tab: "Trophy",
    };
  },
};
</script>
