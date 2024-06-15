<template>
  <div class="price-card">
    <div class="price-card_header">{{ plan }}</div>
    <div class="price-card_price">{{ price }}<sup>$</sup></div>
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(0)"
        />
      </span>
      <span>2 GB of space</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(1)"
        />
      </span>
      <span>14 days of backups</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(2)"
        />
      </span>
      <span>Social integrations</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(3)"
        />
      </span>
      <span>Client billing</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(4)"
        />
      </span>
      <span>Remote access</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(5)"
        />
      </span>
      <span>Custom domain</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(6)"
        />
      </span>
      <span>24 hours support</span>
    </div>
    <!--  -->
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(7)"
        />
      </span>
      <span>Admin tools</span>
    </div>
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(8)"
        />
      </span>
      <span>Collaboration tools</span>
    </div>
    <div class="price-card_option-item">
      <span class="price-card_option-item_icon-container"
        ><v-icon
          icon="fa-check"
          color="green"
          size="x-small"
          v-if="getActiveOptions.includes(9)"
        />
      </span>
      <span>User management</span>
    </div>
    <div class="text-white text-center my-6">
      <v-btn
        rounded="xl"
        size="x-large"
        color="#E93A7D"
        :variant="recommended ? 'flat' : 'outlined'"
        class="text-white"
        >Get Started</v-btn
      >
    </div>
  </div>
</template>
<script setup>
import { defineProps, computed } from "vue";
const props = defineProps({
  plan: {
    type: String,
    default: "starter",
  },
  price: {
    type: String,
    default: "9.99",
  },
  recommended: {
    type: Boolean,
    default: false,
  },
});

const getActiveOptions = computed(() => {
  switch (props.plan) {
    case "starter":
      return [0, 1, 2, 3];
    case "professional":
      return [0, 1, 2, 3, 4, 5, 6];
    case "team":
      return [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
    default:
      break;
  }
});
</script>
<style scoped>
.price-card {
  border: 1px solid gray;
  padding: 44px 50px;
  border-radius: 8px;
}
.price-card_header {
  font-size: 22px;
  padding-left: 18px;
  text-transform: capitalize;
}
.price-card_price {
  font-size: 58px;
  padding-left: 18px;
  margin: 15px 0;
  margin-top: 5px;
}
sup {
  font-size: 16px;
  top: -35px;
  left: 5px;
}
.price-card_option-item {
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  gap: 14px;
  font-size: 16px;
  margin-bottom: 10px;
  font-weight: 300;
}
.price-card_option-item_icon-container {
  min-width: 16px;
  min-height: 16px;
}
</style>
