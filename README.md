ex6.css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
}

header {
    background-color: #f8f8f8;
    padding: 10px 2%;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap; 
}

.navbar-brand {
    display: flex;
    align-items: center;
}

.navbar-brand a {
    font-size: 2rem;
    font-weight: bold;
    color: #000000;
    text-decoration: none;
    margin-left: 10px;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}

.nav-links li {
    position: relative;
}

.nav-links a {
    text-decoration: none;
    color: #333;
    font-weight: 500;
}

.nav-links a:hover,
.nav-links .active {
    color: #d66b00;
    text-decoration: none;
}

.nav-links li span {
    font-size: 0.8rem;
    margin-left: 5px;
}

main {
    background-color: bisque;
    font-size: 1rem;
    padding: 20vh 2%; 
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    color: #222222;
}

main input {
    font-size: 1rem;
}

.container {
    background-color: white;
    border-radius: 15px;
    text-align: center;
    padding: 10%;
    max-width: 75%;
    margin: 0 auto;
    overflow: hidden;
}

.inactive {
    background-color: #ffa449;
    border: #222222 1.5px solid;
    border-radius: 15px;
    padding: 8px;
}

.inactive:hover {
    color: white !important;
    background-color: #fc8005;
}

.submit {
    font-size: 1rem;
    background-color: rgb(255, 136, 92);
    padding: 8px 16px;
    border: #222222 1.5px solid;
    border-radius: 15px;
}

.submit:hover {
    background-color: #fc8005;
    color: white;
    cursor: pointer;
}

.titleForm {
    color: #d66b00;
}

.navbar-brand .logo {
    color: #d66b00;
}

.error {
    color: red;
}

.modal {
    display: none; 
    position: fixed; 
    z-index: 1; 
    left: 0;
    top: 0;
    width: 100%; 
    height: 100%; 
    overflow: auto; 
    background-color: rgba(0, 0, 0, 0.4); 
}

.modal-content {
    background-color: #fefefe;
    margin: 15% auto; 
    padding: 20px;
    border: 1px solid #888;
    border-radius: 15px;
    width: 80%; 
    text-align: center;
}

.close {
    color: #aaa;
    float: right;
    font-size: 28px;
    font-weight: bold;
}

.close:hover,
.close:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
    position: relative;
    bottom: 0;
    width: 100%;
}

footer a {
    color: #ff9100; 
    text-decoration: none;
}
footer a:hover {
    text-decoration: underline;
}
.footer-links {
    margin: 10px 0;
}

/* responsive media */
@media (max-width: 768px) {
    .nav-links {
        flex-direction: column; 
        align-items: center; 
    }
    .nav-links li {
        margin: 10px 0; 
    }
    
    main {
        padding: 10vh 2%; 
    }
    
    .container {
        max-width: 90%; 
    }
}

@media (max-width: 480px) {
    .navbar-brand a {
        font-size: 1.5rem; 
    }
    .submit, .inactive {
        font-size: 0.9rem; 
        padding: 6px 12px; 
    }
    
}
