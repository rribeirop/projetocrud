<%-- 
    Document   : cadastrarCategoria
    Created on : 22/08/2024, 20:58:06
    Author     : Roger
--%>

<%@page contentType="text/html" pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
        <title>Cadastrar Categoria</title>
    </head>
    <body>
        <h1>Cadastrar Categoria</h1>
        <form action="CadastrarAluno">
            <label>ID Categoria: </label>
            <input type="text" name="idCategoria" readonly=""
                   value="${categoria.idCategoria == 0 ? "" : categoria.idCategoria}" >

            <label> Nome Categoria: </label>
            <input type="text" name="nomeCategoria" required=""
                   value="${categoria.nomeCategoria}" >

            <label> Código da Categoria: </label>
            <input type="text" name="codigoCategoria" required=""
                   value="${categoria.codigoCategoria}" >

            <label> Data de Criação: </label>
            <input type="date" name="dataCriacao" required=""
                   value="${categoria.dataCriacao}" >
            
            <label> Valor médio: </label>
            <input type="date" name="valorMedio" required=""
                   value="${categoria.valorMedio}" >

            <button type="submit">Gravar</button>
        </form>
                   
        <p> ${mensagem} </p>
        
    </body>
</html>
