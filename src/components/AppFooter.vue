<template>
    <footer class="app-footer">
        <div class="footer-content">
            <p>&copy; 2025 My Company. All rights reserved.</p>
            <nav class="footer-links">
                <a href="/about">About Us</a>
                <a href="/contact">Contact</a>
                <a href="/privacy">Privacy Policy</a>
            </nav>
        </div>
    </footer>
</template>

<script>
export default {
    name: "AppFooter",
};
</script>

<style scoped>
.app-footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem 0;
    bottom: 0;
    width: 100%;
    margin-top: 90px;
    box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.2);
}

.footer-content {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.footer-links {
    margin-top: 0.5rem;
}

.footer-links a {
    color: #4caf50;
    text-decoration: none;
    margin: 0 0.5rem;
    font-size: 0.9rem;
}

.footer-links a:hover {
    text-decoration: underline;
}
</style>