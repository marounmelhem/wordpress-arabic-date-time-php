# wordpress-arabic-date-time-php
# Author: Maroun Melhem <mm@marounmelhem.com>
# Author URI: http://maroun.me

A simpler method to display wordpress post date and time in arabic for a wordpress website.
Many other methods are available but this one does not include additional libraries and It's clear and simple to use.

Instructions:

**Date:

   1-paste the "single_post_arabic_date" function in your theme's functions.php file
   2-Inside your wordpress loop call the function to display the date using the following method:
   <code>
    <date>
      <?php
        $postdate_d = get_the_date('d');
        $postdate_d2 = get_the_date('D');
        $postdate_m = get_the_date('M');
        $postdate_y = get_the_date('Y');

        echo single_post_arabic_date($postdate_d, $postdate_d2, $postdate_m, $postdate_y);
      ?>
    </date>
   </code 
    
  **Time:
  
   1-paste the "single_post_arabic_time" function in your theme's functions.php file
   2-Inside your wordpress loop call the function to display the time using the following method:
   
   <span>الساعة </span>
     <time>
         <?php
           $posttime_h = get_the_date('h');
           $posttime_i = get_the_date('i');
           $posttime_s = get_the_date('d');
           $posttime_a = get_the_date('A');
           
           echo single_post_arabic_time($posttime_h,$posttime_i,$posttime_a);
          ?>
      </time>
