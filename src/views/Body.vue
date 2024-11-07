<script setup>
import { ref } from 'vue'
import locationIcon from '@/assets/svg/location.svg'
import messageIcon from '@/assets/svg/message.svg'
import linkIcon from '@/assets/svg/link.svg'
import externalLink from '@/assets/svg/el.svg'
import gradIcon from '@/assets/svg/grad.svg'
import headphoneIcon from '@/assets/svg/headphone.svg'

const value = ref(5)
const star4 = ref(3.6)
</script>

<template>
  <div class="base-container">
    <div class="left">
      <Card :title="$t('about.title')">
        {{ $t('about.text') }}
      </Card>
      <Card :title="$t('skills.title')">
        {{ $t('skills.text') }}
        <div class="skills">
          <div class="progress">
            <div class="progress-item">
              <h3 class="bar-heading">Javascript & Nodejs <span>Expert</span></h3>
              <el-progress
                :text-inside="false"
                :stroke-width="15"
                :percentage="90"
                :show-text="false"
                color="#66cb8c"
              />
            </div>
            <div class="progress-item">
              <h3 class="bar-heading">HTML, CSS & SASS <span>Expert</span></h3>
              <el-progress
                :text-inside="false"
                :stroke-width="15"
                :percentage="92"
                :show-text="false"
                color="#66cb8c"
              />
            </div>
            <div class="progress-item">
              <h3 class="bar-heading">Vue, React, Nuxt & Next <span>Pro</span></h3>
              <el-progress
                :text-inside="false"
                :stroke-width="15"
                :percentage="57"
                :show-text="false"
                color="#66cb8c"
              />
            </div>
            <div class="progress-item">
              <h3 class="bar-heading">Python & AHK <span>Pro</span></h3>
              <el-progress
                :text-inside="false"
                :stroke-width="15"
                :percentage="75"
                :show-text="false"
                color="#66cb8c"
              />
            </div>
          </div>
          <a href="https://github.com/EjazEkay"><externalLink />{{ $t('skills.more') }}</a>
        </div>
      </Card>
      <Card :title="$t('language.title')">
        <div class="lang-container">
          <div class="lang-item">
            <p>
              Urdu: <span>{{ $t('language.type1') }}</span>
            </p>
            <el-rate :colors="['#66CB8C', '#66CB8C', '#66CB8C']" v-model="value" allow-half disabled />
          </div>
          <div class="lang-item">
            <p>
              Saraiki: <span>{{ $t('language.type1') }}</span>
            </p>
            <el-rate :colors="['#66CB8C', '#66CB8C', '#66CB8C']" v-model="value" allow-half disabled />
          </div>
          <div class="lang-item">
            <p>
              English: <span>{{ $t('language.type2') }}</span>
            </p>
            <el-rate :colors="['#66CB8C', '#66CB8C', '#66CB8C']" v-model="star4" allow-half disabled />
          </div>
        </div>
      </Card>
    </div>
    <div class="right">
      <Card>
        <div class="info">
          <p><locationIcon />{{ $t('location') }}</p>
          <a :href="$t('mail.mailto')"><messageIcon />{{ $t('mail.address') }}</a>
          <a :href="$t('github.url')" target="_blank"><linkIcon />{{ $t('github.url') }}</a>
        </div>
      </Card>
      <Card :title="$t('education')">
        <div class="edu-container">
          <div class="edu-item">
            <h4><gradIcon />BSc Computer Science</h4>
            <p>Qurtuba University <span>(2020-2024)</span></p>
          </div>
        </div>
      </Card>
      <Card :title="$t('music')">
        <div class="listmusic">
          <p><headphoneIcon />Mustafa Jan-E-Rehmat Pay Lakhon Salam</p>
          <p><headphoneIcon />Maikada 3 (Bus Ik Nigah)</p>
          <p><headphoneIcon />Wo Jali Hai Ya Khafi Hai</p>
        </div>
      </Card>
    </div>
  </div>
</template>

<style scoped>
.listmusic p {
  display: flex;
  gap: 10px;
  align-items: center;
  color: var(--subtitle);
  font-size: 16px;
  line-height: 20px;
}

.listmusic {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.lang-container {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.lang-item span {
  font-weight: 400;
}

.lang-item p {
  font-size: 16px;
  font-weight: 700;
}

.lang-item {
  display: flex;
  flex-direction: column;
  color: var(--title);
  font-family: var(--font-title);
}

.edu-item {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.edu-item h4 {
  color: var(--title);
  display: flex;
  gap: 5px;
}

.edu-item p {
  color: var(--dimmed);
  margin-left: 25px;
  font-family: var(--font);
  font-weight: 700;
  font-size: 14px;
}

.edu-item span {
  font-weight: 400;
}

.base-container {
  margin-top: 48px;
  margin-bottom: 76px;
  display: flex;
  flex-direction: column;
  gap: 24px;
  max-width: 768px;
}

.left {
  display: flex;
  flex-direction: column;
  gap: 30px;
  width: 66.66666667%;
  width: 100%;
}
.right {
  display: flex;
  flex-direction: column;
  gap: 30px;
  width: 33.33333333%;
  width: 100%;
}

.info {
  display: flex;
  flex-direction: column;
  gap: 12px;
}

.info a,
.info p {
  display: flex;
  gap: 12px;
  width: fit-content;
}

.skills {
  display: flex;
  flex-direction: column;
}

.skills a {
  gap: 6px;
  line-height: 16px;
  display: flex;
}

.skills .progress {
  margin-bottom: 30px;
  display: flex;
  flex-direction: column;
  gap: 30px;
}

.skills .progress-item {
  width: 100%;
}

.bar-heading {
  display: flex;
  font-size: 16px;
  font-weight: 700;
  font-family: var(--font-title);
  color: var(--title);
  margin-bottom: 8px;
}

.bar-heading span {
  margin-left: auto;
  font-family: var(--font);
  font-size: 16px;
  font-weight: 400;
  color: #ccd1d6;
}

@media (min-width: 960px) {
  .base-container {
    flex-direction: row;
    max-width: 1360px;
  }
  .left {
    width: 66.66666667%;
  }
  .right {
    width: 33.33333333%;
  }
}
</style>
