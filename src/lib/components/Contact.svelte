<script lang="ts">
    let name = ''
    let email = ''
    let message = ''

    async function handleSubmit() {
        const formData = { name, email, message }

        try {
        } catch (error) {
            console.error('Error sending message:', error)
        }
    }
</script>

<div class="rounded-md p-6 shadow-md">
    <h2 class="mb-4 text-2xl font-semibold underline">Contact:</h2>
    <form on:submit={handleSubmit}>
        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700 dark:text-white" for="name">Name:</label>
            <input placeholder="Name" class="w-full rounded border bg-indigo-200 dark:bg-slate-500 py-2 px-3 text-slate-700 dark:text-white" type="text" id="name" bind:value={name} />
        </div>
        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700 dark:text-white" for="email">Email:</label>
            <input
                placeholder="email@gmail.com"
                class="w-full rounded border bg-indigo-200 dark:bg-slate-500 py-2 px-3 text-slate-700 dark:text-white"
                type="email"
                id="email"
                bind:value={email}
            />
        </div>

        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700 dark:text-white" for="message">Message:</label>
            <textarea
                placeholder="Write your message here"
                class="w-full rounded border bg-indigo-200 dark:bg-slate-500 py-2 px-3 text-slate-700 dark:text-white"
                id="message"
                bind:value={message}
            />
        </div>
        <div class="flex justify-center">
            <button class="rounded bg-indigo-600 py-2 px-8 font-bold text-white hover:bg-indigo-800" type="submit"> Send </button>
        </div>
    </form>
</div>
