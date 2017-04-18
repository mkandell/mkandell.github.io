# mkandell.github.io
Website Portfolio

<!DOCTYPE html>
<!--[if lt IE 8 ]><html class="no-js ie ie7" lang="en"> <![endif]-->
<!--[if IE 8 ]><html class="no-js ie ie8" lang="en"> <![endif]-->
<!--[if (gte IE 8)|!(IE)]><!--><html class="no-js" lang="en"> <!--<![endif]-->
<head>

   <!--- Random Stuff
   ================================================== -->
   <meta charset="utf-8">
   <meta name="description" content="">
   <meta name="author" content="">
   <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">

   <!--- Title
   ================================================== -->

   <!-- TODO: Change this to change the label displayed at the top of the website (look at the tab!) -->
	<title>
            Website 101: Build Your Own Portolio Website in Two Hours
   </title>

	<!-- CSS
    ================================================== -->
   <!-- GOOD TO KNOW: This loads up what is known as a "stylesheet", essentially where all your CSS rules will go. The "href" attribute tells our file where to search for our stylesheets. Here it's saying "Start at where our file is located in our current folder and go into the css folder and find *.css. Then load it up."-->
   <link rel="stylesheet" href="css/default.css">
	<link rel="stylesheet" href="css/layout.css">
   <link rel="stylesheet" href="css/media-queries.css">
   <link rel="stylesheet" href="css/magnific-popup.css">

   <!-- Script
   ================================================== -->
	<!-- GOOD TO KNOW: This does the same thing as above except it instead loads a "script". A script, in this case, is what a file with jQuery code is called. On a side note, jQuery is a Javascript library (library = a set of pre-written code that some really really smart people wrote and allowed us all to use for free) that allows you to make edits to the html elements we have on this page. jQuery is often used to make websites interactive; this is what causes the website to scroll when you click on a link or change color when you're hovering over something. This won't be covered in the context of this workshop but if you want to make your website more interactive, learning jQuery can help you out! If you want to see a simple example of how jQuery works, open up js/init.js and check it out.-->
   <script src="js/modernizr.js"></script>

   <!-- Favicons
	================================================== -->
   <!-- TODO: Look at the image that looks like a C at the top of your webpage near the title (look at the tab name). Currently, the picture that is being stored is the same as the picture stored in the same folder that this file is stored in under the name "favicon.png" (which is why the href attribute is equal to that). You can either choose to change that href attribute to point to your own custom picture (by dropping your picture into the folder this file is located in and changing the href attribute's value to point to that), or omit this following code entirely if you don't want to use an icon. 

   Note: if this is not displaying for you, try using a browser like Chrome! Browsers like Safari don't show this at the top-->
	<link rel="shortcut icon" href="favicon.png" >

</head>

<body>

   <!-- Header
   ================================================== -->
   <header id="home">

      <nav id="nav-wrap">

         <a class="mobile-btn" href="#nav-wrap" title="Show navigation">Show navigation</a>
	      <a class="mobile-btn" href="#" title="Hide navigation">Hide navigation</a>

         <!-- TODO: The following <li class="itemAtTop"> elements are what are displayed on the top of your page. If you want to change the text that is displayed on top, simply replace the text. If you want to change which element is highlighted at the beginning, make the initially highlighted <li> element the one that has class="itemAtTop current", since this tells the CSS stylesheets to apply different rules (i.e. coloring and stuff) to only the element with this class. If you want to change which div the elements lead to when they are clicked, change the href attribute to #{the id of the div you want it linked to} (i.e. #home). If you want to create more of these, simply copy and paste the li element.-->

         <!-- TODO: This TODO is a continuation of a TODO listed below in the resume section, on adding new sections to your resume. IGNORE THIS IF YOU HAVE NOT REACHED THAT POINT YET!

         Continuing from before, copy and paste any of the <li> elements in your desired position. For example, if you want to create your new button after General, copy and paste this belownGeneral:

         <li class="itemAtTop">
            <a class="smoothscroll" href="#home">
               General
            </a>
         </li>
   
         Note: make sure to make the class attribute class="itemAtTop" instead of
         class="itemAtTop current", unless you want this to be the initially selected element.

         Now change General to whatever text you want and make the href attribute #{the id you selected in the initial part}. Now refresh the page and it should work for you.

         -->

         <ul id="nav" class="nav">
            <li class="itemAtTop current">
               <a class="smoothscroll" href="#home">
                  General
               </a>
            </li>
            <li class="itemAtTop">
               <a class="smoothscroll" href="#about">
                  About Me
               </a>
            </li>
            <li class="itemAtTop">
               <a class="smoothscroll" href="#education">
                  Education
               </a>
            </li>
            <li class="itemAtTop">
               <a class="smoothscroll" href="#work">
                  Work
               </a>
            </li>
            <li class="itemAtTop">
               <a class="smoothscroll" href="#skills">
                  Skills
               </a>
            </li>
         </ul> <!-- end #nav -->

      </nav> <!-- end #nav-wrap -->


      <div class="row banner">
         <div class="banner-text">

            <!-- TODO: Change the text -->

            <h1 class="responsive-headline">
               I'm Maya Kandell.
            </h1>

            <!-- TODO: Change the text. If you want to change which words are highlighted white, move around the <span> </span> elements. If you want to have one of the words link to another part of this website, wrap it with:

            <a class="smoothscroll" href='#{div id}'>TEXT</a>

            If you want to have one of the words link to another website, omit the class="smoothscroll" and just insert the raw link as the value for the href attribute.

            For example, if you want to link to Google.com, then the following link would work:

            <a href="google.com"> TEXT </a>

            -->

            <h3>
               I'm a <span>Silicon Valley</span> based <span>illustrator</span> and <span>artist</span> creating independent projects and commissioned works for clients all over the United States. Let's <a class="smoothscroll" href="#about">start scrolling</a>
               and learn more <a class="smoothscroll" href="#about">about me</a>.
            </h3>

            <!-- GOOD TO KNOW: This just creates a horizontal bar. -->
            <hr />

            <!-- TODO: These are the social media buttons linked on the page. To make these link to something, just replace the href="#" with href="YOUR LINK HERE". Also, feel free to delete any of these if you don't need them.

            Also, if you want the link to open on a different page, add in the target="_blank" attribute to your <a> elements. This will tell the HTML to load up your link in a different page. -->

            <!-- GOOD TO KNOW: If you want to use any different logos than the ones available here, there are a lot of additional logos available in css/font-awesome/css/font-awesome.css. To try them out just replace the existing fa-whatever in the <i> element's class attribute to whatever you can find in that file (note: that file will have period before the actual name of the class like .fa-{whichever icon you choose} since in CSS the preceding period denotes an HTML class). If you want to find additional ones, look at the FontAwesome library of icons online, which is where these current ones come from! -->
            <ul class="social">
               <li>
                  <a href="#" target="_blank">
                     <i class="fa fa-facebook"></i>
                  </a>
               </li>
               <li>
                  <a href="#" target="_blank">
                     <i class="fa fa-twitter"></i>
                  </a>
               </li>
               <li>
                  <a href="#" target="_blank">
                     <i class="fa fa-google-plus"></i>
                  </a>
               </li>
               <li>
                  <a href="#" target="_blank">
                     <i class="fa fa-linkedin"></i>
                  </a>
               </li>
               <li>
                  <a href="#" target="_blank">
                     <i class="fa fa-instagram"></i>
                  </a>
               </li>
            </ul>
         </div>
      </div>

      <!-- GOOD TO KNOW: This is what creates the arrow that automatically scrolls to the about section. Feel free to change the href to a different part of the page if you would like. -->

      <p class="scrolldown">
         <a class="smoothscroll" href="#about"><i class="icon-down-circle"></i></a>
      </p>

   </header> <!-- Header End -->


   <!-- About Section
   ================================================== -->
   <div id="about">

      <div class="row">

         <div class="three columns">

            <!-- TODO: To edit the existing clock image, simply change the src attribute to the path to the picture you want. Right now, the src attribute is telling our file to go to the current folder that our file is located in, find the images folder, and search for "sample-image.jpg" within it 

            If you want to have your website display some alternative text in case it can't display this image for some reason, set the text you want it to display inside the alt attribute.-->

            <img class="profile-pic"  src="images/sample-image.jpg" alt="" />

         </div>

         <div class="nine columns main-col">

            <!-- TODO: Change text-->
            <h2>
               About Me
            </h2>

            <!-- TODO: Change text-->
            <p>
               I'm a UC Berkeley student studying Global Development, and taking art classes on the side. My passions include drawing gnomes, reading, engaging in friendly arguments with people about politics, and learning about global poverty. 
            </p>

            <div class="row">

               <div class="columns contact-details">

                  <!-- TODO: Change text-->
                  <h2>
                     Contact Details
                  </h2>

                  <!-- TODO: Change text.-->
                  <p class="address">

						   <span>
                        Maya Kandell
                     </span>

                     <!-- GOOD TO KNOW: The <br> element tells the html to leave an empty line.-->
                     <br>

						   <span>
                        427 Lotus Lane
                        <br>
						      Mountain View, CA 94043 US
                     </span>

                     <br>

                     <!-- TODO: Change text. Also, "mailto:" and "tel:" let the html file to automatically email or call the following email or number, so make sure to change the corresponding href attribute to follow with the number that you change! -->

						   <span>
                        <a href="tel:1234567890">
                           (650) 575-1387
                        </a>
                     </span>

                     <br>
                     
                     <span>
                        <a href="mailto:anyone@website.com">
                           mkandell@berkeley.edu
                        </a>
                     </span>
					   </p>

               </div>

               <div class="columns download">
                  <p>
                     <!-- TODO: Change the text and the icon if you want. See the stuff written above with the social media buttons to change the icon. 

                     Also, change the href="index.html" attribute to a link to your resume. Right now when you click on it it will download this file (index.html), but if instead you upload your resume to the folder in which this file is contained and insert its name (i.e. JohnDoeResume.pdf) as the value of the href element, it will create a download link for your resume instead.
                     -->
                     <a href="Maya'sResume.pdf" class="button" download>
                        <i class="fa fa-download"></i>Download Resume
                     </a>
                  </p>
               </div>
                     <a href="APportfolio.zip" class="button" download>
                        <i class="fa fa-download"></i>Download Portfolio
                     </a>
                  </p>
               </div>

            </div> <!-- end row -->

         </div> <!-- end .main-col -->

      </div>

   </div> <!-- About Section End-->


   <!-- Resume Section
   ================================================== -->

   <!-- TODO:

        If you want to add another section, on top of Education, Work, and Skills, there is a multistep process involved in doing so.

        1) Copy everything from <div class="resume" id="education"> to </div>. When you are doing this, be very careful to stop at the correct </div>. The correct </div> will be the first </div> element that lines up vertically with <div class="resume" id="education">, so be very careful when you're doing this. Refresh your page once you have done this to make sure it works.

        2) Change <div class="resume" id="education"> to <div class="resume" id={INSERT AN ID HERE}>. Your id can be anything you want; however, the id that you pick at this point will be what you use above in order to make sure that the page scrolls to the right section when you implement smooth-scroll later on.

        3) Scroll up all the way to the top to where you defined General, About Me, Education, Work, and Skills. The instructions on how to add scrolling functionality to scroll down to this section from the top will be explained there in more detail. But make sure you keep track of the id that you used!

   -->

   <div class="resume" id="education">

      <!-- Education -->
      <div class="row">

         <div class="three columns header-col">
            <!-- TODO: Change text, if you want. -->
            <h1>
               <span>
                  Education
               </span>
            </h1>
         </div>

         <div class="nine columns main-col">

            <div class="row item">

               <div class="twelve columns">

                  <!-- TODO: Change text. -->
                  <h3>
                     University of California, Berkeley
                  </h3>

                  <!-- GOOD TO KNOW: &bull; creates a bullet point in HTML. There are a couple more of these HTML Special Symbol you can put in; search it up if you want a different one! Also, the <em> tag usually "emphasizes" a particular element. In this case, its used as a way to remove the font styling put on anything with the class "info", which our <p> element currently has. -->
                  <!-- TODO: Change text. -->
                  <p class="info">

                     BA in Development Studies 

                     <span>
                        &bull;
                     </span> 

                     <em class="date">
                        May 2020
                     </em>
                  </p>

                  <!-- TODO: Change text. -->
                  <p>
                  Undergraduate degree in Development Studies, a venture in order to make mself a global citizen and hopefully a little more interesting. Oh, and also a way of learning more about how to make the world a better place. I'm taking a number of Art Practice classes and elective art classes along the way in order to expand my creative toolbox. 
                  </p>

               </div>

            </div> <!-- item end -->

            <!-- GOOD TO KNOW:
            If you want to add more experiences, copy EVERYTHING from:

            <div class="row item"> 

            to the first:

            </div>

             -->

         </div> <!-- main-col end -->

      </div> <!-- End Education -->
      
   </div>

   <div class="resume" id="work">
      <!-- Work -->

      <div class="row">

         <!-- TODO: Change the text and stuff, just as above. -->

         <div class="three columns header-col">
            <h1>
               <span>
                  Work
               </span>
            </h1>
         </div>

         <div class="nine columns main-col">

            <div class="row item">

               <div class="twelve columns">

                  <h3>
                     Independent Sticker Business
                  </h3>

                  <p class="info">
                     CEO, Captain, Her Majesty, etc.

                     <span>&bull;</span> 

                     <em class="date">
                        March 2017 - Present
                     </em>
                  </p>

                  <p>
                  Creates whimsical illustrations in spare moments, alters them in such a way so that they are suitable as stickers, and markets products on Etsy using social media outlets and advertising expertise gained from former internships. 
                  </p>

               </div>

            </div> <!-- item end -->

         </div> <!-- main-col end -->

      </div> <!-- End Work -->

   </div>

   <div class="resume" id="skills">

      <!-- Skills -->
      <div class="row">

         <!-- TODO: Change the text and stuff, just as above. -->

         <div class="three columns header-col">
            <h1>
               <span>
                  Skills
               </span>
            </h1>
         </div>

         <div class="nine columns main-col">

            <p>
               I have significant experience with the design-oriented members of the Adobe Suite — InDesign through my years as a magazine editor, photoshop through my time as an illustrator, and Illustrator due to my brief ventures into making vector t-shirt designs. 
            </p>

            <!-- TODO: To change the name of the skill, just change the white text within the <em> tags. To change the width of the bar displayed, simply edit the style attribute of the <span> to be "width={your percent}%"-->

				<div class="bars">

				   <ul class="skills">
					   <li>
                     <em>Photoshop</em>
                     <span style="width:80%" class="bar-expand"></span>
                  </li>
                  <li>
                     <em>Illustrator</em>
                     <span style="width:50%" class="bar-expand"></span>
                  </li>
						<li> 
                     <em>InDesign</em>
                     <span style="width:95%" class="bar-expand"></span>
                  </li>
                  <li>
                     <em>Adobe Audition</em>
                     <span style="width:85%" class="bar-expand"></span>    
				</div><!-- end skill-bars -->

			</div> <!-- main-col end -->

      </div> <!-- End skills -->

   </div> <!-- Resume Section End-->


   <!-- footer
   ================================================== -->
   <footer>

      <div class="row">

         <div class="twelve columns">

            <!-- TODO: Change the href attributes to link to your social media sites and change the class to reflect the icon you want to choose. See the information written in this file above regarding social media website buttons for more information on what to do! --> 
            <ul class="social-links">
               <li><a href="#"><i class="fa fa-facebook"></i></a></li>
               <li><a href="#"><i class="fa fa-twitter"></i></a></li>
               <li><a href="#"><i class="fa fa-google-plus"></i></a></li>
               <li><a href="#"><i class="fa fa-linkedin"></i></a></li>
               <li><a href="#"><i class="fa fa-instagram"></i></a></li>
               <li><a href="#"><i class="fa fa-dribbble"></i></a></li>
               <li><a href="#"><i class="fa fa-skype"></i></a></li>
            </ul>

            <!-- GOOD TO KNOW: the &copy; is another example of an HTML Special Symbol. Search them up if you are interested!

            Also, the following snippet is from the original creator of this design, Styleshout. We made heavy modifications to their design to bring the one in front of you today. Legally, you might be required to leave this on your site, so remove at your own risk. --> 
            <ul class="copyright">
               <li>&copy; Copyright 2014 CeeVee</li>
               <li>Design by <a title="Styleshout" href="http://www.styleshout.com/">Styleshout</a></li>   
            </ul>

         </div>

         <!-- GOOD TO KNOW: This is the button that takes up to the top of the page. -->
         <div id="go-top"><a class="smoothscroll" title="Back to Top" href="#home"><i class="icon-up-open"></i></a></div>

      </div>

   </footer> <!-- Footer End-->

   <!-- Java Script
   ================================================== -->
   <!-- GOOD TO KNOW: This does the same thing as above except it instead loads a "script". A script, in this case, is what a file with jQuery code is called. On a side note, jQuery is a Javascript library (library = a set of pre-written code that some really really smart people wrote and allowed us all to use for free) that allows you to make edits to the html elements we have on this page. jQuery is often used to make websites interactive; this is what causes the website to scroll when you click on a link or change color when you're hovering over something. This won't be covered in the context of this workshop but if you want to make your website more interactive, learning jQuery can help you out! If you want to see a simple example of how jQuery works, open up js/init.js and check it out.-->
   <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
   <script>window.jQuery || document.write('<script src="js/jquery-1.10.2.min.js"><\/script>')</script>
   <script type="text/javascript" src="js/jquery-migrate-1.2.1.min.js"></script>

   <script src="js/jquery.flexslider.js"></script>
   <script src="js/waypoints.js"></script>
   <script src="js/jquery.fittext.js"></script>
   <script src="js/magnific-popup.js"></script>
   <script src="js/init.js"></script>

</body>

</html>
