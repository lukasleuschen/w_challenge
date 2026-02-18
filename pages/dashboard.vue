<script setup lang="ts">
import AnalyticsAward from '@/views/dashboard/AnalyticsAward.vue';
import AnalyticsTransactions from '@/views/dashboard/AnalyticsTransactions.vue';
import AnalyticsWeeklyOverview from '@/views/dashboard/AnalyticsWeeklyOverview.vue';
import AnalyticsTotalEarning from '@/views/dashboard/AnalyticsTotalEarning.vue';
import AnalyticsBarCharts from '@/views/dashboard/AnalyticsBarCharts.vue';
import AnalyticsTotalProfitLineCharts from '@/views/dashboard/AnalyticsTotalProfitLineCharts.vue';
import AnalyticsUserTable from '@/views/dashboard/AnalyticsUserTable.vue';
import AnalyticsSalesByCountries from '@/views/dashboard/AnalyticsSalesByCountries.vue';
import AnalyticsDepositWithdraw from '@/views/dashboard/AnalyticsDepositWithdraw.vue';
import AnalyticsTotalProfit from '@/views/dashboard/AnalyticsTotalProfit.vue';
import AnalyticsNewProject from '@/views/dashboard/AnalyticsNewProject.vue';

</script>

<template>
    <VRow class="match-height">
      <VCol
        cols="12"
        md="4"
      >
        <AnalyticsAward />
      </VCol>
      <VCol>
        <AnalyticsTransactions />
      </VCol>
    </VRow>
    <VRow>
      <VCol cols="12" md="4">
        <AnalyticsWeeklyOverview />
      </VCol>
      <VCol cols="12" md="4">
        <AnalyticsTotalEarning />
      </VCol>
      <VCol cols="12" md="4">
        <VRow>
          <VCol>
            <AnalyticsTotalProfitLineCharts />
          </VCol>
          <VCol>
            <AnalyticsTotalProfit />
          </VCol>
        </VRow>
        <VRow>
          <VCol>
            <AnalyticsNewProject />
          </VCol>
          <VCol>
            <AnalyticsBarCharts />
          </VCol>
        </VRow>
      </VCol>
    </VRow>
    <VRow  class="match-height">
      <VCol cols="12" md="4">
        <AnalyticsSalesByCountries />
      </VCol>
      <VCol>
        <AnalyticsDepositWithdraw />
      </VCol>
    </VRow>
    <VRow  class="match-height">
      <VCol cols="12">
        <AnalyticsUserTable />
      </VCol>
    </VRow>
</template>
