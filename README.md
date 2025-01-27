/* Resetando margens e paddings para evitar inconsistências */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Definindo o estilo do body e fonte padrão */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f4f4f4;
}

/* Cabeçalho e navegação */
header {
    background-color: #333;
    color: white;
    padding: 10px 0;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style-type: none;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Hero Section */
.hero {
    text-align: center;
    padding: 50px 20px;
    background-color: #007BFF;
    color: white;
}

/* Seção de conteúdo */
.content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
}

.content article {
    background-color: white;
    padding: 20px;
    margin: 10px;
    width: 30%;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.content article h2 {
    margin-bottom: 10px;
}

.content article p {
    font-size: 14px;
    color: #555;
}

/* Rodapé */
footer {
    text-align: center;
    background-color: #333;
    color: white;
    padding: 20px;
}

/* Media Queries para Responsividade */

/* Para telas menores que 768px (como tablets e smartphones em paisagem) */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
    }

    .content {
        flex-direction: column;
        align-items: center;
    }

    .content article {
        width: 80%;
    }
}

/* Para telas menores que 480px (como smartphones em retrato) */
@media (max-width: 480px) {
    .hero {
        padding: 30px 15px;
    }

    .content article {
        width: 100%;
    }

    footer {
        padding: 10px;
    }
}
