<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import PrimaryButton from '../../Components/PrimaryButton.vue';

defineProps({
    mustVerifyEmail: {
        type: Boolean,
    },
    status: {
        type: String,
    },
});
</script>

<template>
    <Head title="Settlement" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Settlement</h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8 space-y-6">
                <div class="p-4 sm:p-8 bg-white shadow sm:rounded-lg">
                    <PrimaryButton>
                        <a href="/payment/linepay/geturl/1" target="_blank">LINE Payで支払う</a>
                    </PrimaryButton>

                </div>

                <div class="p-4 sm:p-8 bg-white shadow sm:rounded-lg">
                    
                </div>


            </div>
        </div>
    </AuthenticatedLayout>
</template>
