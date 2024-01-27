<script setup>
import TaskList from '@/components/TaskList.vue';
import AddTask from '@/components/AddTask.vue';
import ControlPanel from '@/components/ControlPanel.vue';
</script>

<template>
    <div class="container">
        <h1>Task list</h1>
        <div class="view-content">
            <AddTask />
            <ControlPanel />
            <TaskList />
        </div>
    </div>
</template>

<style scoped lang="scss">
.view-content {
    max-width: 600px;
    margin: 0 auto 12px;
    @include flex($fd: column, $ai: normal);
    gap: $common-gap;
}
</style>
