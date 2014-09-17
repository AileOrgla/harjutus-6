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
    		echo "<br>";
    	?>
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
    		echo "<br>";
    	?>
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
   </body>

</html>
