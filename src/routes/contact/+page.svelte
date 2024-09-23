<script>
    export let title = "Contact Me";
</script>

<style>
    main {
        padding: 30px;
        min-height: calc(100vh - 140px); 
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: white;
        box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        border-radius: 12px;
        margin: 20px;
    }

    h1 {
        font-size: 2.5rem;
        margin-bottom: 20px;
    }

    p {
        font-size: 1.2rem;
        margin: 10px 0;
    }

    a {
        color: #4a90e2;
        text-decoration: none;
        font-weight: bold;
    }

    a:hover {
        text-decoration: underline;
    }


    .social-links {
        display: flex;
        gap: 15px;
        margin-top: 20px;
    }

    .social-icon {
        width: 30px;
        height: 30px;
    }

  
    .profile-image {
        width: 100px; 
        height: 100px; 
        border-radius: 50%; 
        object-fit: cover; 
        margin-bottom: 20px; 
        border: 2px solid #4a90e2; 
    }
</style>

<main>
    <img class="profile-image" src="https://scontent.fmnl9-4.fna.fbcdn.net/v/t39.30808-6/417700330_2565452523618014_1754247105946385500_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=127cfc&_nc_eui2=AeErtPp0xQ-EPDDkvz3JR7fg4Kz20DFuIbfgrPbQMW4htygqCYGEIGRL7pErtwifGwQhozL4kcYgGULLQH4kmMBd&_nc_ohc=6-8lwXReKiIQ7kNvgHFyGa3&_nc_ht=scontent.fmnl9-4.fna&_nc_gid=AU0BO-751In2KxXB6wsg4UK&oh=00_AYAJRGhKC19LNLbTJgRr3LPH7vMQoQ1D7lQ8Z-BsJRN6bg&oe=66F70A3A" alt="Profile Picture" />
    <h1>{title}</h1>
    <p>If you'd like to get in touch, feel free to reach out through any of the following platforms:</p>

    <p>
        Email: 
        <a href="https://mail.google.com/mail/?view=cm&fs=1&to=202210145@gordoncollege.edu.ph" target="_blank">
            202210145@gordoncollege.edu.ph
        </a>
    </p>
    

    <div class="social-links">
        <a href="https://github.com/cryzii-6" target="_blank">
            <img class="social-icon" src="https://img.icons8.com/material-outlined/24/4a90e2/github.png" alt="GitHub" />
        </a>
        <a href="https://facebook.com/crz.ynn" target="_blank">
            <img class="social-icon" src="https://img.icons8.com/material-outlined/24/4a90e2/facebook.png" alt="Facebook" />
        </a>
        <a href="https://instagram.com/_cryzii" target="_blank">
            <img class="social-icon" src="https://img.icons8.com/material-outlined/24/4a90e2/instagram-new.png" alt="Instagram" />
        </a>
        <a href="https://linkedin.com/in/ynnyannah-vea-cruz-10817432b" target="_blank">
            <img class="social-icon" src="https://img.icons8.com/material-outlined/24/4a90e2/linkedin.png" alt="LinkedIn" />
        </a>
    </div>
</main>
