<script>
    export let title = "Personal Story: Ynnyannah's Life";
</script>

<style>
    body {
        margin: 0;
        font-family: 'Arial', sans-serif;
        background: linear-gradient(135deg, #74ebd5, #ACB6E5); 
        color: #333;
        overflow-x: hidden; 
    }

    header {
        background-color: rgba(74, 144, 226, 0.9); 
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
        text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5)
    }

    main {
        padding: 30px; 
        min-height: calc(100vh - 180px);
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: white;
        box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        border-radius: 12px;
        margin: 20px;
        transition: all 0.3s ease; 
    }

    footer {
        background-color: #333;
        color: white;
        text-align: center;
        padding: 10px;
        position: relative;
        width: 100%;
        bottom: 0;
        margin-top: 20px; 
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
            padding: 20px; 
        }
    }
</style>

<header>
    <h1>{title}</h1>
</header>

<main>
    <slot />
</main>

<footer>
    <p>&copy; 2024 Personal Story: Ynnyannah's Life. All rights reserved.</p>
</footer>
