# ELF
Il s'agit là dans un premier temps de reproduire la commande readelf et finalement faire la fusion de deux fichiers objets au format ELF32 bits.
Ce projet vise à utiliser les pointeurs en C et aussi exploiter une grosse doctumentation technique en Anglais. Pour mieux comprendre le linker ELF il faut se référer aux documents sur internet.
<ul>
  <li><b>Compilation<b><br/>
    Pour obtenir les deux exécutables <code>readelf</code> et <code>myld</code> il faut se placer dans le réportoire principale sous la console et faire:</br>
    <ul>
      <li>chmod u+x configure</li>
      <li>./configure</li>
      <li>make</li>
    </ul>    
  </li>
  <li><b>Utilisation des programmes</b>
      <ol>
        <li> ./readelf -options(-h,-S,-x N° ou -x noms,-s,-a) nom_fichier</li>
        <li>./myld fichier1.o fichier2.o fichier_resultat</li>
      </ol>
   </li>
  <li><b>Tests et scripts</b><br/>
    Deux scripts shell sont utilisés pour automatiser les tests et pour exécuter il faut faire :
    <ul>
      <li>chmod +x Scripts_tests/test_content_section.sh</li>
      <li>chmod +x Scripts_tests/test_h_s.sh</li>
      <li>./Scripts_tests/test_h_s.sh options</li>
    </ul>
  </li>
</ul>
