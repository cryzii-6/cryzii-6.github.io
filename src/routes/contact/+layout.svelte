<script>
    export let title = "Contact Page";
</script>

<style>
    body {
        margin: 0;
        font-family: 'Arial', sans-serif;
        background: linear-gradient(135deg, #74ebd5, #ACB6E5); /* Beautiful gradient */
        color: #333;
        overflow-x: hidden; /* Prevent horizontal scroll */
    }

    header {
        background-color: rgba(74, 144, 226, 0.9); /* Semi-transparent background */
        color: white;
        padding: 20px;
        text-align: center;
        box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
        border-radius: 8px;
        margin: 20px;
    }

    h1 {
        margin: 0;
        font-size: 2.5rem;
        text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5); /* Subtle shadow for depth */
    }

    main {
        padding: 30px; /* Increased padding for better spacing */
        min-height: calc(100vh - 180px); /* Adjusted height for footer */
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: white;
        box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        border-radius: 12px;
        margin: 20px;
        transition: all 0.3s ease; /* Smooth transitions */
    }

    footer {
        background-color: rgba(74, 144, 226, 0.9); /* Matches header color */
        color: white;
        text-align: center;
        padding: 10px;
        position: relative;
        width: 100%;
        bottom: 0;
        margin-top: 20px; /* Added margin for spacing */
    }

    p {
        margin: 0;
    }

    @media (max-width: 600px) {
        h1 {
            font-size: 2rem;
        }

        main {
            margin: 10px;
            padding: 20px; /* Adjusted padding for smaller screens */
        }
    }
</style>

<header>
    <h1>{title}</h1>
</header>

<main>
    <slot /> <!-- This is where your page content will be injected -->
</main>

<footer>
    <p>&copy; 2024 Ynnyannah Vea Cruz BSIT 3C. All rights reserved.</p>
</footer>
