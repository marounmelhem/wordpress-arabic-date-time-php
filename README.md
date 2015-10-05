# wordpress-arabic-date-time-php
# Author: Maroun Melhem <mm@marounmelhem.com>
# Author URI: http://maroun.me

A simpler method to display wordpress post date and time in arabic for a wordpress website.

Many other methods are available but this one does not include additional libraries and It's clear and simple to use.

Instructions:

**Date:<br/><br/>
   1-paste the "single_post_arabic_date" function in your theme's functions.php file<br/>
   2-Inside your wordpress loop call the function to display the date using the following method:<br/><br/>
   <pre>
      <?php
        $postdate_d = get_the_date('d');<br/>
        $postdate_d2 = get_the_date('D');<br/>
        $postdate_m = get_the_date('M');<br/>
        $postdate_y = get_the_date('Y');<br/>
        echo single_post_arabic_date($postdate_d, $postdate_d2, $postdate_m, $postdate_y);
      ?>
   </pre> 
    
  **Time:<br/><br/>
   1-paste the "single_post_arabic_time" function in your theme's functions.php file<br/>
   2-Inside your wordpress loop call the function to display the time using the following method:<br/><br/>
   <pre><br/>
         <?php
           $posttime_h = get_the_date('h');<br/>
           $posttime_i = get_the_date('i');<br/>
           $posttime_s = get_the_date('d');<br/>
           $posttime_a = get_the_date('A');<br/>
           echo single_post_arabic_time($posttime_h,$posttime_i,$posttime_a);
          ?>
   </pre>
