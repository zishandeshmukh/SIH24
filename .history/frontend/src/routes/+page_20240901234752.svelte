<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Custom Tailwind Example</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@latest/dist/tailwind.min.css" rel="stylesheet">
    <style>
        :root {
            --font-heading: 'Arial, sans-serif'; /* Example heading font */
            --font-body: 'Courier New, monospace'; /* Example body font */
            --border: 210, 16%, 93%; /* Example HSL value */
            --input: 210, 16%, 96%; /* Example HSL value */
            --ring: 210, 16%, 85%; /* Example HSL value */
            --background: 210, 16%, 98%; /* Example HSL value */
            --foreground: 210, 10%, 23%; /* Example HSL value */
            --primary: 220, 90%, 56%; /* Example HSL value */
            --primary-foreground: 220, 90%, 96%; /* Example HSL value */
            --secondary: 340, 65%, 47%; /* Example HSL value */
            --secondary-foreground: 340, 85%, 97%; /* Example HSL value */
            --destructive: 10, 75%, 52%; /* Example HSL value */
            --destructive-foreground: 10, 85%, 97%; /* Example HSL value */
            --muted: 210, 10%, 80%; /* Example HSL value */
            --muted-foreground: 210, 10%, 20%; /* Example HSL value */
            --accent: 45, 100%, 51%; /* Example HSL value */
            --accent-foreground: 45, 100%, 98%; /* Example HSL value */
            --popover: 210, 16%, 98%; /* Example HSL value */
            --popover-foreground: 210, 10%, 23%; /* Example HSL value */
            --card: 0, 0%, 100%; /* Example HSL value */
            --card-foreground: 0, 0%, 0%; /* Example HSL value */
            --radius: 12px; /* Example radius */
        }

        /* Accordion animations */
        @keyframes accordion-down {
            from { height: 0; }
            to { height: var(--radix-accordion-content-height); }
        }

        @keyframes accordion-up {
            from { height: var(--radix-accordion-content-height); }
            to { height: 0; }
        }

        .accordion-down {
            animation: accordion-down 0.2s ease-out;
        }

        .accordion-up {
            animation: accordion-up 0.2s ease-out;
        }
    </style>
</head>
<body class="bg-background text-foreground font-body">
    <!-- Example Heading -->
    <h1 class="font-heading text-primary">Welcome to the Custom Tailwind Page</h1>

    <!-- Example Input Field -->
    <input class="border border-border p-2 rounded-md" placeholder="Type something..." />

    <!-- Example Card -->
    <div class="bg-card text-card-foreground p-4 rounded-lg shadow-lg mt-4">
        <p>This is an example card component.</p>
    </div>

    <!-- Example Button -->
    <button class="bg-primary text-primary-foreground px-4 py-2 rounded-md mt-4">
        Click Me
    </button>

    <!-- Accordion Example -->
    <div class="accordion mt-6">
        <button class="accordion-trigger p-2 bg-secondary text-secondary-foreground rounded-lg w-full">
            Toggle Accordion
        </button>
        <div class="accordion-content hidden overflow-hidden">
            <p class="p-4">This is the content of the accordion.</p>
        </div>
    </div>

    <script>
        // Example accordion toggle logic
        document.querySelector('.accordion-trigger').addEventListener('click', function () {
            const content = document.querySelector('.accordion-content');
            if (content.classList.contains('hidden')) {
                content.classList.remove('hidden');
                content.classList.add('accordion-down');
                content.style.height = `${content.scrollHeight}px`;
            } else {
                content.classList.add('accordion-up');
                content.style.height = '0px';
                setTimeout(() => content.classList.add('hidden'), 200);
            }
        });
    </script>
</body>
</html>
