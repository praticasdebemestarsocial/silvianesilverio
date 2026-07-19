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
    function traduzirNosDeTexto(node) {
        if (node.nodeType === Node.TEXT_NODE) {
            let original = node.nodeValue;
            let traduzido = original
                .replace("Contact Information", "Contato")
                .replace("Name", "Nome")
                .replace("Professional Title", "Profissão")
                .replace("Education", "Educação (Graduação e Pós)")
                .replace("Experience", "Experiência Profissional")
                .replace("Certificates", "Cursos de Formação e Eventos")
                .replace("Awards", "Congressos e Seminários");
            
            if (original !== traduzido) {
                node.nodeValue = traduzido;
            }
        } else {
            // Percorre os filhos recursivamente
            node.childNodes.forEach(traduzirNosDeTexto);
        }
    }
    
    // Inicia a varredura dentro da área principal da página
    const contentDiv = document.querySelector('article');
    if (contentDiv) {
        traduzirNosDeTexto(contentDiv);
    }
});
</script>
