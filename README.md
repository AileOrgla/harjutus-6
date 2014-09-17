harjutus-6
==========
<!DOCTYPE HTML>
<html>
   <head>
   <title>Harjutus3</title>
   <meta http-equiv="Content-Type" content="text/html;
   charset=utf-8">
   <title>PHP põhitõed</title>
   </head>
   <body>
      <h2>Tingimuslaused</h2>
      	<?php
      		$a = 4;
      		$b = 5;
      		if ($a<$b) {
      			echo "$a on väiksem kui $b";
      		}
      	?>
      	<?php
      		$a = 6;
      		$b = 3;
      		if ($a<$b) {
      			echo "$a on väiksem kui $b";
      		}
      	?>
      	<?php
      		if ($b < $a) {
      			// Kuna see on tõene, siis väljastatakse see tekst.
        		echo "$b on väiksem kui $a";
    		} elseif ($a = $a) {
        		// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$a on $a";
    		} elseif ($b > $a) {
    			// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$a on suurem kui $b";      
    		}
    	?>
    	<br>
    	<?php
    		$a = 5;
      	$b = 5;
      		if ($b < $a) {
      			// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$b on väiksem kui $a";
    		} elseif ($a = $a) {
        		// Kuna see on tõene, siis väljastatakse see tekst.
        		echo "$a on $b";
    		} elseif ($b > $a) {
    			// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$a on suurem kui $b";      
    		}
    	?>
    	<br>
    	<?php
    		$a = 7;
      	$b = 2;
      		if ($b < $a) {
      			// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$b on väiksem kui $a";
    		} elseif ($a = $a) {
        		// Kuna see ei ole tõene, siis ei väljastata seda teksti.
        		echo "$a on $b";
    		} elseif ($b > $a) {
    			// Kuna see on tõene, siis väljastatakse see tekst.
        		echo "$a on suurem kui $b";      
    		}
    	?>
    	<br>
      <?php
        $age = 18;
        $age_limit = 18;
          if ($age >= $age_limit) {
              echo "Olete piisavalt vana. Tulge edasi!";
            } elseif ($age < $age_limit) {
              echo "Kahjuks olete liiga noor.Te peate olema vähemalt $age_limit aastat vana. Tulge n aasta pärast tagasi.";
        }
      ?>
      <br>
    	<?php
        $a = 3;
        $b = 3;
        $c = 4;
        $d = 5;

          if (($a = $b) && ($c > $d)) {
              echo "Esimene ning teine muutuja on võrdsed ja kolmas muutuja on suurem kui neljas.";
              // Antud koodiplokk ei käivitunud, kuna esimene ning teine muutuja on võrdsed, aga kolmas muutuja ei ole suurem, kui neljas. Selleks, et käivitus, peavad mõlemad tõesed olema.
            }
          if (($a = $b) || ($c > $d)) {
              echo "Üks komponentlausetest on õige.";
              // Vähemalt üks komponentlausetest on tõene (esimene muutuja on võrdne teisega) ning seepärast koodiblokk käivitatakse.
        }
      ?>
      <br>
      <?php
        if (isset($nothing)==false) {
            echo "Käivitab.";
          }
        if (!isset($nothing)==false) {
            echo "Ei käivita.";
        }
        if (!isset($nothing)==true) {
            echo "Käivitab.";
        }
      ?>
      <h3>Switch</h3>
        <?php
          $current_language = "fi";

          switch ($current_language) {
              case "et":
                echo "Tere! Kuidas sul läheb?";
                break; 
              case "ru":
                echo "Здравствуйте! Как вы делаете?";
                break;
              case "fi":
                echo "Hei! Miten menee?";
                break;
              default:
                echo "Hello! How are you?";
          }
        ?>
   </body>

</html>
