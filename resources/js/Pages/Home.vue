<template>
    <CustomLayout title="Home">
        <div>
            <div class="p-4">
                <div class="bg-white p-4 rounded-md">
                    <div>
                        <h2 class="mb-4 text-xl font-bold text-gray-700">Posts</h2>
                        <div>
                            <div>
                                <div
                                    class="grid grid-cols-4 gap-4 bg-gradient-to-tr from-indigo-600 to-purple-600 rounded-md py-2 px-4 text-white font-bold text-md">
                                    <div>
                                        <span>ID#</span>
                                    </div>
                                    <div>
                                        <span>Title</span>
                                    </div>
                                    <div>
                                        <span>Content</span>
                                    </div>
                                </div>
                                <div v-for="post in posts" :key="post.id">
                                    <div class="grid grid-cols-4 gap-4 border-t-2 text-sm font-normal mt-4">
                                        <div>
                                            <span>{{ post.id }}</span>
                                        </div>
                                        <div>
                                            <span>{{ post.title }}</span>
                                        </div>
                                        <div>
                                            <span>{{ post.content }}</span>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </CustomLayout>
</template>

<script setup>
import CustomLayout from '../Layouts/CustomLayout.vue';
defineProps({
    posts: Object,
});
</script>

<style lang="css" scoped></style>