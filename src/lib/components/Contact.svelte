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
    <h2 class="mb-4 text-xl font-semibold">Contact Me</h2>
    <form on:submit={handleSubmit}>
        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700" for="name">Name:</label>
            <input
                placeholder="Alex Paz"
                class="w-full rounded border py-2 px-3 text-slate-700 bg-slate-500"
                type="text"
                id="name"
                bind:value={name}
            />
        </div>
        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700" for="email">Email:</label>
            <input
                placeholder="email@gmail.com"
                class="w-full rounded border py-2 px-3 text-slate-700 bg-slate-500"
                type="email"
                id="email"
                bind:value={email}
            />
        </div>
        <div class="mb-4">
            <label class="mb-2 block text-sm font-bold text-slate-700" for="message">Message:</label>
            <textarea
                placeholder="Write your message here"
                class="w-full rounded border py-2 px-3 text-slate-700 bg-slate-500"
                id="message"
                bind:value={message}
            />
        </div>
        <button class="rounded bg-indigo-600 py-2 px-4 font-bold text-white hover:bg-indigo-800" type="submit">
            Send
        </button>
    </form>
</div>
