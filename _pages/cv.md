---
layout: cv
permalink: /cv/
title: Currículo
nav: true
nav_order: 5
cv_pdf: # você pode adicionar um link para baixar o seu PDF aqui depois
cv_format: rendercv
description: Este é o meu currículo completo, contendo todas as minhas qualificações, cursos e experiências profissionais.
toc:
  sidebar: left
---

<style>
/* Torna a foto de perfil redonda */
img[src*='foto_perfil.jpg'] {
    border-radius: 50% !important;
    width: 150px !important;
    height: 150px !important;
    object-fit: cover !important;
    margin: 0 auto;
    display: block;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}
</style>

<script>
// Traduz os termos em inglês do layout padrão do currículo
document.addEventListener("DOMContentLoaded", function() {
    const translations = {
        "Contact Information": "Informações de Contato",
        "Name": "Nome",
        "Professional Title": "Título Profissional",
        "Email": "E-mail",
        "Education": "Educação (Graduação e Pós)",
        "Experience": "Experiência Profissional",
        "Certificates": "Cursos de Formação e Eventos",
        "Awards": "Congressos e Seminários"
    };

    // Percorre todos os títulos e células de tabela
    document.querySelectorAll("h3, h2, th, td, span").forEach(el => {
        const text = el.innerText.trim();
        if (translations[text]) {
            el.innerText = translations[text];
        }
    });
});
</script>
