<head>
<title>DHow To Sell Drugs Online (Fast) VOSTFR</title>
  <script type="text/javascript"
   src="/js/jquery.js"></script>
</head>
<body>
<h1>How To Sell Drugs Online (Fast) VOSTFR 6 Episodes | Saison 1</h1>
<b><div style="font-weight:bold;color:#ff0000">How To Sell Drugs Online (Fast) VOSTFR 6 Episodes | Saison 1</div></b>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?8ldt04qd86491zgerfl9&af=2579981">Episode 1</a></b><br>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?yn3niwlavadoxyxq9eds&af=2579981">Episode 2</a></b><br>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?kegdtx9ee09xt3ybo2jf&af=2579981">Episode 3</a></b><br>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?3dv4cighukw6k9ibcinj&af=2579981">Episode 4</a></b><br>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?v73v8b8iu43dnvrb6zwp&af=2579981">Episode 5</a></b><br>
<b><a rel="external nofollow" target="_blank" href="https://1fichier.com/?d2hh76ht3b3ce8qdged6&af=2579981">Episode 6</a></b><br>
<br/>
  <form action="?id=commentaire" method="post" id="form">
 <fieldset>
    <legend>Ajouter un commentaire</legend> 
    <label for="pseudo">Pseudo</label>
      <input type="text" name="pseudo" id="pseudo" />
    <br />
    <label for="contenu">Commentaire</label>
      <textarea name="contenu" id="contenu" rows="4" cols="4"></textarea> 
    <br />
    <input type="submit" value="Ok" />
 </fieldset>
 </form>
 <div id="commentaire">
    <p class="last pair first" id="com_1"><strong>BN</strong> a dit :<br />Coucou !  Je m'appelle BN et je suis un BN, et toi, tu fais quoi dans la vie ?</p>
 </div>
$(document).ready(function() {
    // Au submit du formulaire
    $('#form').submit( function() {
        var pseudo = $('#pseudo').val();
        var commentaire = $('#contenu').val();
        // On supprime les anciens messages d'erreurs ou de succès
        $('.erreur').remove();
        $('.ok').remove();
        // Si on a commentaire à ajouter
        if (pseudo != '' && commentaire != '') {
            // On compte le nombre de commentaire déjà présent + celui qui va être créé
            var nbCom=1;
            $('#commentaire p').each(function() { nbCom++; });
            // On enlève la class "last" à l'ancien dernier
            $('.last').removeClass('last');
            // On ajoute le nouvel élément
            $('#commentaire').prepend('<p class="last" id="com_'+nbCom+'"><strong>'+pseudo+'</strong> a dit :<br />'+commentaire+'</p>');
            // On le met pair ou impair
            if ($('.last').next().is('.pair'))
                $('.last').addClass('impair');
            else
                $('.last').addClass('pair');
            if (!$('.last').next().is('p'))
                $('.last').addClass('first');
            // On efface le contenu du formulaire
            $('#contenu').val('').focus();
            $('#contenu').after('<span class="ok">Commentaire ajouté avec succès</span>');
            $('.ok').hide().fadeIn('slow');
        }       else {
            if (pseudo == '')
                $('#pseudo').after('<span class="erreur">Champ requis</span>');
            if (commentaire == '')
                $('#contenu').after('<span class="erreur">Champ requis</span>');
            $('.erreur').hide().fadeIn('slow');
        }
        // On retourne false pour ne pas recharger la page
        return false;
    });
});
</body>
