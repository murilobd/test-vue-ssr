<template>
  <div class="about">
    <h1>{{ $t('title_about_page') }}</h1>
    <pre>
      Current locale is: {{ currentLocale }}
    </pre>
    <div>
      <select name="locale" id="locale" v-model="currentLocale">
        <option value="en">English</option>
        <option value="fr">French</option>
      </select>
    </div>
  </div>
</template>

<script>
import i18n from "@/i18n";
export default {
  computed: {
    currentLocale: {
      get() {
        return i18n.locale;
      },
      set(_newLocale) {
        i18n.locale = _newLocale;
      }
    }
  }
}
</script>