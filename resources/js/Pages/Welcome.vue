<script setup>
import { Head, Link } from '@inertiajs/vue3';
import Tweet from '@/Components/Tweet.vue';
import TwitterLayout from '@/Layouts/TwitterLayout.vue';

</script>

<template>
    <Head title="Welcome" />

    <TwitterLayout>
        <div class="text-white">
            <div class="flex">
                <Tweet :tweet="{
                    name: 'Johnni Ward',
                    handle: '@johnniward',
                    image: 'https://randomuser.me/api/portraits/men/40.jpg',
                    tweet: 'We went rock climbing this weekend? Here is the video. Climbing is way more fun than exercising on any gym equipment. It works both your mind and body',
                    file: '/videos/Sportsman.mp4',
                    is_video: true,
                    comments: '35',
                    retweets: '54',
                    likes: '88',
                    analytics: '81',
                }" />
            </div>
            <div class="border-b border-b-gray-800 mt-2"></div>
        </div>
    </TwitterLayout>
</template>
