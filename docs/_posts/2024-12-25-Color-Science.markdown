
---
layout: post
title:  "Color"
date:   2024-12-25 11:56:33 +0530
categories: Neuroscience
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Color Science</title>
    <style>
        
        .container {
            position: relative;
            width: 100px;
            height: 100px;
            margin-bottom: 20px;
            /* left: 30%; */
        }

        .circle {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            display: none;  /* Initially hide all circles */
            position: absolute;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #4CAF50;
            color: white;
            border: none;
            /* position:relative; */
            left: 30%;
            border-radius: 5px;
            margin-top: 10px;
        }

        button:hover {
            background-color: #45a049;
        }

        #result {
            margin-top: 20px;
            font-size: 18px;
        }
    
    
        /* Basic CSS for layout similar to Jekyll default */
        
        header h1 {
            font-size: 3.5rem;
            margin: 0;
        }

        header p {
            margin-top: 0.5rem;
            font-size: 1.2rem;
        }

        

        article h2 {
            font-size: 2.2rem;
            margin-bottom: 1rem;
        }
        article h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        article time {
            font-size: 0.9rem;
            color: #888;
            margin-bottom: 1.5rem;
            display: block;
        }

        article p {
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 1.5rem;
            width: 950px;
        }

        .content {
            padding-bottom: 2rem;
            
        }
        .quote-container {
            margin-left: 50px; /* Adds an offset to the left */
            font-style: italic; /* Italicizes the quote */
            font-size: 1.0em; /* Increases font size */
            color: #555; /* Sets a subtle text color */
            border-left: 4px solid #888; /* Adds a left border for emphasis */
            padding-left: 20px; /* Adds space between the border and the text */
            line-height: 1.6; /* Increases line height for readability */
            max-width: 80%; /* Limits the width of the quote */
            margin-top: 30px; /* Adds margin on top */
            width : 800px;
        }
        
        .quote-author {
            text-align: right; /* Right-aligns the author's name */
            font-weight: bold; /* Makes the author's name bold */
            margin-top: 10px; /* Adds a bit of space after the quote */
            font-size: 1.2em; /* Slightly smaller font size for the author */
            color: #333; /* Darker color for the author's name */
        }

        .footer {
            text-align: center;
            padding: 1rem;
            background-color: #333;
            color: #fff;
            margin-top: 2rem;
        }

        
        /* Link styles */
        a {
            color: #007bff;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        


        /* Media queries for responsiveness */
        @media (min-width: 768px) {
            .content {
                display: flex;
                gap: 2rem;
            }

            .main-content {
                flex: 1;
            }

            .sidebar {
                flex: 0 0 250px;
            }
        }
        .color-display {
            width: 300px;
            height: 300px; /* Full height for the circle */
            position: relative;
            left: 30%;
            margin-bottom: 20px;
            overflow: hidden; /* Hide overflow for semicircles */
        }
        .semicircle {
            width: 100%;
            height: 50%; /* Each semicircle occupies half the height */
            position: absolute;
            left: 0;
        }
        .semicircle_top {
            top: 0; /* Position at the top */
            background-color: rgb(0, 0, 0); /* Placeholder for random color */
            border-top-left-radius: 150px; /* Round top left corner */
            border-top-right-radius: 150px; /* Round top right corner */
        }
        .semicircle_bottom {
            bottom: 0; /* Position at the bottom */
            background-color: rgb(127, 127, 127); /* Default color */
            transition: background-color 0.2s;
            border-bottom-left-radius: 150px; /* Round bottom left corner */
            border-bottom-right-radius: 150px; /* Round bottom right corner */
        }
        .horizontal-line {
            position: absolute;
            top: 50%; /* Center the line vertically */
            left: 0;
            width: 100%;
            height: 10px; /* Height of the line */
            background-color: black; /* Color of the line */
            transform: translateY(-50%); /* Adjust for line height */
        }
        .slider {
            width: 100;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            margin-top: 10px;
            cursor: pointer;
        }

    </style>
</head>
<body>
    
    <!-- Main Content Area -->
    <main>
        <div class="content">
            <!-- Blog Post Section -->
            <div class="main-content">
                <article>
                    <h1>Color Science: Predicting Biology from Behavior</h1>
                    <!-- <time datetime="2024-11-17">November 17, 2024</time> -->
                    
                    <p> In Ted Chiang&#39;s <a href='https://www.lightspeedmagazine.com/fiction/exhalation/'>Exhalation</a>, a mechanical being notices that their species&#39; perception of time has sped up and suspects that this is because their brains have gotten slower. 
                        They then build an intricate device that lets them peer inside their own brain and observe the machinery that gives rise to their thoughts: 
                        a  complex engine at the center of which was a latticework of wires with gold leaves held in various positions based on an ever-changing pattern of air flow.
                         They deduce that &#39;<i>All that we are is a pattern of air flow&#39;</i>. The slowing down of their brains was due to an increase in the air pressure of their surroundings. 
                        Following that line of thinking, they arrive at the conclusion that eventually the difference in air pressure between their brains and surroundings will be equalized. When that happens, their thoughts will cease altogether. </p>
                    <p>I love the image that Exhalation conjures of a person observing their own brain in action. But something else that struck me about this story was how their initial hunch came not from looking inside the brain, but by observing their own behavior and their environment. 
                        Centuries before we invented fMRI machines, stuck electrodes inside the brains, or engineered proteins to make the brain glow, scientists made unreasonably accurate predictions about how our brains work. 
                        They did this by making careful observations of the world around us, introspecting on their own experiences and behavior, and through rigorous reasoning. 
                        This post is about one example of the boldness of predicting biology from behavior: the science of color vision. </p>
                    <p>We know that most humans are &#39;trichromats&#39;. Our eyes have three color receptors that are sensitive to different wavelengths of light 
                        and this gives rise to our ability to perceive color. But how exactly did scientists figure this out? </p>
                    
                    
                    <h2 id="studying-the-stimulus-what-is-light-">Studying the stimulus: What is light?</h2>
                    <p><a href="https://www.nobelprize.org/prizes/physics/2024/press-release/">All Physicists are simply future neuroscientists</a>. Newton was no different. </p>
                    <p>To understand how looking at light gives rise to the perception of color, we need to first understand what light is. Newton did a series of elegant experiments to understand the fundamental components of light. </p>
                    
                    <p><img src="images/newton_setup.png" style="width:700px;" alt = 'Newton prism color splitting experiment setup '></p>
                    
                    <div class="quote-container">"As the Rays <span class="hljs-keyword">of</span> light differ <span class="hljs-keyword">in</span> degrees <span class="hljs-keyword">of</span> Refrangibility, so they also differ <span class="hljs-keyword">in</span> their disposition to exhibit this <span class="hljs-keyword">or</span> <span class="hljs-keyword">that</span> particular colour (...) Some Rays are disposed to exhibit a red colour <span class="hljs-keyword">and</span> no other; some a yellow <span class="hljs-keyword">and</span> no other, some a green <span class="hljs-keyword">and</span> no other, <span class="hljs-keyword">and</span> so <span class="hljs-keyword">of</span> the rest" (Opticks, 1704)
                    </div><p>He let sunlight in through a tiny hole in his dark room. He placed a prism in the path of the light and let the refracted light fall upon the screen. Light passed through the prism and formed a rainbow on his screen. He noted that different rays of light differ in how they were refracted, and that the degree of their refractiveness corresponded to the color in which they appeared. </p>
                    <p> Side note: If you're curious about exactly why this happens, I recommend checking out this video by 3blue1brown. </p>
                    
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/KTzGBJPuJwM" frameborder="0" allowfullscreen></iframe>

                    <!-- <img src="images/prism.png" style="width:700px;" alt = 'Dark side of the moon'> -->
                    <p>Then, Newton cut a slit on the screen to allow only a portion of the rainbow to pass through. He placed a second prism in the path of this ray.  He observed that:  </p>
                    
                        <div class="quote-container">
                            "The color <span class="hljs-keyword">of</span> the light was never changed <span class="hljs-keyword">in</span> the least. If any part <span class="hljs-keyword">of</span> the red light was refracted, it remained totally <span class="hljs-keyword">of</span> the same red color <span class="hljs-keyword">as</span> before. No orange, no yellow, no green <span class="hljs-keyword">or</span> blue, nor other new color was produced <span class="hljs-keyword">by</span> <span class="hljs-keyword">that</span> refraction."
                    
                        </div>
                    <p>Newton&#39;s prism had split light into its fundamental components. He then used lenses to converge the rays that passed through the first prism. He observed that he could get back the original light, suggesting that the decomposition of light was reversible. </p>
                    <p>But the part that Newton had not considered was the relationship between the wavelength of the ray of light and what it means for it to appear a certain color to humans. </p>
                    <!-- <p>[Side note: You can do this experiment yourself at home!]</p> -->
                    <h2 id="studying-behavior-metamers">Studying behavior: Metamers</h2>
                    <div class="quote-container">"There <span class="hljs-keyword">is</span> no red <span class="hljs-keyword">in</span> a 700 nm light, just <span class="hljs-keyword">as</span> there <span class="hljs-keyword">is</span> no pain <span class="hljs-keyword">in</span> the hooves <span class="hljs-keyword">of</span> a kicking horse." - Steven Shevell. 
                    </div><p>Color is in the eye of the beholder. Or, more accurately, in the brain of the beholder. This insight was crucial in uncovering the biological basis for color vision. It shifted the emphasis from looking outwards, only studying light itself, to looking inwards and studying the system that is doing the actual perceiving. It might seem obvious, but most things that are obvious in hindsight were nothing but when they were first discovered!</p>
                    <p>People have spent a long time wondering about  <a href="https://en.wikipedia.org/wiki/Knowledge_argument">what it means to experience color</a> and  <a href="https://ismy.blue/">whether my blue is the same as your blue</a>. Newton and others had helped provide an understanding of the basics of how light worked, but for a long time, we still lacked the tools to study the physiology of the eye. How then to get any insight about what gives rise to the perception of color? </p>
                    <p>Newton&#39;s work showed us that sunlight is made up of spectral components of different wavelengths. Early theories suggested that the eye contained &#39;retinal elements&#39; that vibrated in response to light stimulation, and these vibrations helped us see. But if light was made of infinitely many rays of different wavelengths, were there infinitely many retinal elements that each respond to a given wavelength? </p>
                    <p>Thomas Young, amongst other &#39;future neuroscientists&#39; including Helmholtz, Maxwell, and Grassman, was one of the first to propose that there were only three distinct receptor types in the retina. The basis of their assertion was a set of neat behavioral results in what we now call &#39;color-matching&#39; experiments. </p>
                    <p>They presented a person of normal color vision with a &#39;test&#39; light made up of some arbitrary spectral composition. Then, they asked the person to &#39;match&#39; the appearance of the test color by adjusting the intensity of a set of lights with fixed spectral distributions - called primarily lights. </p>
                    
                    <div class="color-display" id="colorDisplay">
                        <div class="semicircle semicircle_top" id="leftSemicircle"></div>
                        <div class="semicircle semicircle_bottom" id="rightSemicircle"></div>
                        <div class="horizontal-line"></div> <!-- Horizontal line -->
                    </div>
                
                    <label for="red">A</label>
                    <input type="range" id="red" class="slider" min="0" max="255" value="127">
                    <span id="redValue">127</span>
                
                    <label for="green">B</label>
                    <input type="range" id="green" class="slider" min="0" max="255" value="127">
                    <span id="greenValue">127</span>
                
                    <label for="blue">C</label>
                    <input type="range" id="blue" class="slider" min="0" max="255" value="127">
                    <span id="blueValue">127</span>
                
                    <button id="randomizeButton">Randomize Color</button> <!-- New button -->
                    
                    <p>They found that having two primary lights was insufficient to match all colors, while having four was too many. These behavioral experiments proved that it was necessary and sufficient to have three appropriately chosen primary lights to match the appearance of <em>any</em> light of arbitrary spectral composition. 
                    This meant that there were infinitely many lights with different spectral distributions that all appeared identical to humans. </p>
                    <p>To illustrate this, look outside your window at the sunlight. Okay, now look at this photo of the sky: </p>
                    <p><img src="images/sun_image.png" style="width:700px;" alt = 'Photo of the sun'></p>

                    <p>In these two cases, your eyes were stimulated by light with very different spectral power distributions. Below, the left panel shows an approximation of the spectral power of the sun. On the right is the spectral distribution of the light coming out of a typical computer monitor which has been calibrated to produce an image that is identical to sunlight to most human observers. Such stimuli, that are physically different but perceptually indistinguishable, are called Metamers. </p>
                    <p><img src="images/sun_spectral_distribution.png" style="width:700px;" alt = 'Spectral power distribution of the sun and its image on a display monitor'><br>From foundations of vision, chapter 4</p>

                    <p>Disclaimer: The color-matching demo above is misleading. We cannot perform a true trichromatic color matching experiment on a computer monitor. 
                        The reason for that is evidence of the enormous impact that this behavioral finding has had on the larger world: 
                        most displays are built with only three different types of phosphors that emit light of particular spectral distributions. 
                        By adjusting the relative intensity of the three lights, we can produce the percept of any color. 
                        But a picture of sunlight on a display monitor is only a metamer of the sunlight we see outside our window. 
                        The science of human color perception made the engineering of these devices possible. (And the International Commission on Illumination codified these standards in 1931, years before we actually measured cells in the eye!)</p>
                    <!-- <p>Imagine that we were only born with two cones instead of three. We can do an analogous version of the color-matching experiment on our computer monitors to get the intuition:</p>
                    <p>{Add demonstration}</p> -->

                    <p>The scientists of the 1800s didn&#39;t just stop at identifying the number of distinct primary lights required to match human vision, but also made precise predictions of &#39;color-matching functions&#39;: the intensity of each chosen primary light needed to match a monochromatic light of a given wavelength. For example, to get a monochromatic light of wavelength 550nm, what we need is an intensity of 1 for R, intensity of 1 for G, and intensity of 0 for B. </p>
                    <p><img src="images/color_matching_functions.png" style="width:700px;" alt = 'Color matching functions based on human psychophysics'></p>

                    <p>The color matching functions are not unique: So if we used two distinct sets of primary lights, we will arrive at different color-matching functions. But the two functions are related by a linear transformation. We can think of this linear transformation as adjusting the intensities of the first set of primary lights to match the intensities of the second set of primary lights. </p>
                    <p>Based on these findings, they predicted that the human eye must contain three types of receptors. Moreover, they predicted that the absorption spectra of these three receptors must explain the color-matching results, i.e. they will be related to the color-matching functions by a linear transformation. </p>
                    <p>This was all figured out by the 1850s. It took us more than a hundred years after that to actually test and verify these predictions by studying the properties of photoreceptors in the human eye! </p>
                    <h2 id="studying-physiology-cones">Studying Physiology: Cones</h2>
                    <div class="quote-container">To suppose that <span class="hljs-keyword">the</span> eye <span class="hljs-keyword">with</span> all its inimitable contrivances <span class="hljs-keyword">for</span> adjusting <span class="hljs-keyword">the</span> focus <span class="hljs-built_in">to</span> different distances, <span class="hljs-keyword">for</span> admitting different amounts <span class="hljs-keyword">of</span> light, <span class="hljs-keyword">and</span> <span class="hljs-keyword">for</span> <span class="hljs-keyword">the</span> correction <span class="hljs-keyword">of</span> spherical <span class="hljs-keyword">and</span> chromatic aberration, could have been formed <span class="hljs-keyword">by</span> natural selection, seems, I freely confess, absurd <span class="hljs-keyword">in</span> <span class="hljs-keyword">the</span> highest degree - Charles Darwin.
                    </div>
                    <br>
                    <p><img src="images/davinci_eye.png" style="width:400px;" alt = 'Da Vinci drawing of the eye'></p>

                    <p>To conclude the saga and discover the biological basis of human trichromatic vision, in the late 1900s, Baylor, Nunn, and Schnapf painstakingly measured the spectral sensitivities of the different cone types. To do this, they harvested retinas, the sheet of tissue at the back of the eye where light falls. Our retina contains primarily two types of photo-receptors: Rods and Cones. When light falls on these cells, they convert this to electrical signals. Rods operate more in &#39;scotopic&#39; vision, that is when it is relatively dark. Cones operate in photopic vision, when it is bright, and mediate &#39;color vision&#39; because there are three types of cones that are sensitive to different wavelengths. The fact that there are three types of cones, was known by the 1980s. But their exact spectral sensitivities, that is the shape and amplitude of how much each wavelength of light excites a given cone, had not been measured. These measurements are key in testing whether the cone spectral sensitivites can explain the behavioral results from the color-matching experiments.</p>
                    <p>So, Baylor and colleagues undertook this heroic experiment. They took the harvested retinal tissue, isolated a single cone, and preserved it in a solution that keeps it alive for a few hours post-harvesting. Then, they passed monochromatic lights of various wavelengths and observed the sensitivity of different cones. They found three different cone types with spectral response functions that showed peaks in different wavelengths, which they called the short, medium, and long wavelength cones. Further, they  showed that there is a linear transformation that converts the cone photocurrent measurements into the color-matching functions predicted from the behavioral experiments. This paper finally provided the biological basis to explain the results from the color-matching experiments. </p>
                    <p><img src="images/cone_spectral_sensitivity.png" style="width:400px;" alt = 'Cone spectral sensitivity'></p>

                    
                    <p>I first learned about this from <a href = "https://www.cns.nyu.edu/~eero/">Eero Simoncelli</a> when I attended the <a href = "https://meetings.cshl.edu/courses.aspx?course=c-visi">CSHL course on vision</a>. Here's a quote from a <a href="https://www.youtube.com/watch?v=eKKXJyabCAQ">talk</a> of his where he does a much better job of conveying the essence of this scientific story and why it&#39;s worthy of praise. (In his own career, he sought to and succeeded in discovering a similar scientific story: <a href='https://pubmed.ncbi.nlm.nih.gov/21841776/'>Metamers and pattern vision</a> )</p>
                    <div class="quote-container">"It's amazing <span class="hljs-keyword">that</span> you can have a theory <span class="hljs-keyword">and</span> a <span class="hljs-keyword">set</span> <span class="hljs-keyword">of</span> behavioral experiments <span class="hljs-keyword">that</span> make very precise <span class="hljs-keyword">and</span> clear predictions <span class="hljs-keyword">that</span> get verified <span class="hljs-keyword">and</span> tested <span class="hljs-keyword">in</span> a mechanistic sense almost a hundred years later."
                    
                    
                    </div><h2 id="studying-others-what-we-cannot-see">Studying others: Predicting Behavior from Biology</h2>
                    <p>So far, we&#39;ve talked about a story of the triumph of behavioral science in predicting biology. But often, scientific progress comes from an <a href="https://buzsakilab.com/wp/2019/02/06/the-brain-from-inside-out-by-buzsaki-g/">Inside-Out</a> approach - studying biology to predict psychology. I&#39;ll write about one such case that I first came across in Ed Yong's book 'An Immense World'. </p>
                    <p>Once scientists established that normal human vision is trichromatic and that the biological basis for this is the three types of cones we have, they started to look for situations where this was <em>not</em> the case. Color-blindness is one obvious example that people were aware of for centuries (Maxwell, one of the protagonists of the color-matching experiments, wrote extensively about its implication for color-blindness). But what of those that can see more than I can? </p>
                    <p> <a href='https://research.ncl.ac.uk/tetrachromacy/'>Gabriele Jordan and colleagues</a> are interested in whether there may be tetrachromats hiding amongst us - humans with four distinct cones who are able to perceive colors that are identical to most of us trichromats. But searching for tetrachromacy is not easy for a variety of reasons. For one, they might not even realize their perception is different! </p>
                    <p>Instead of hoping that the tetrachromats will self-identify and call up their nearest color researcher, these scientists put together a set of conditions to narrow the search down. The key to figuring out the right set of conditions lies in understanding the genetics behind cone cells.</p>
                    
                    <p>First, it's far more likely that a female is tetrachromatic compared to a male.
                         It is also more likely that a male has color-vision deficits compared to a female.
                         This is because the genes that determine the properties of your cones is in your X chromosome. 
                         So it's possible for females to inherit both an X-chromosome with the typical S, M, L cone genes and the other X-chromosome with a wonky copy of, say, the M-cone gene such that this cone responds to a slightly different wavelength compared to typical human M-cones. But how to narrow down which females to study to find tetrachromacy? The key is to look at the mothers/daughters of males who exhibit a specific type of color deficiency called "anamalous trichromacy" that is easier to spot behaviorally . An anamalous trichromat has an M or L cone with slightly shifted wavelength preferences. The mother/daughter of an anamalous trichromat is an 'obligate carrier' of this spectrally shifted hybrid cone, in addition to having the standard S, M, and L cones. </p>

                    <p>So these researchers put out TV ads to recruit boys who are anamlous trichromats and their mothers to participate in their study. Having these four cones is a necessary but not sufficient condition for exhibiting behavioral tetrachromacy. A few more conditions need to be met:  the extra cone needs to be responsive to a very specific wavelength, it has to be abundant in the part of the retina that perceives information in the fovea, i.e. the central portion of our visual field, and perhaps the most complicated requirement, the brain needs to be able to process its responses to actually use the information the fourth cone relays to give rise to perception. </p> 
                    <p>The researchers narrowed down their list to twenty four eligible mothers and had them do a behavioral experiment called the Rayleigh Discrimination Test. </p>
                    <p>They presented three colored circles in quick succession. Two of the three circles were made of monochromatic light of wavelength 590nm. The other circle was a mixture of two lights: Red (670nm) and Green (546nm). The order of presentation of the three circles is randomized each time and the participant must guess which of the three was the mixture circle. For participants with normal trichromatic vision, for certain ratios of R and G, the mixture circle will appear to be identical to the monochromatic circle. This is the essence of the color-matching behavioral experiments we previously spoke about. However, if a person has a fourth cone that had a preferred wavelength of XX and they were able to use the signals from that cone for perception, they might be able to tell apart colors that are identical to others.</p>
                    
                    <div class="container">
                        <div class="circle" id="circle1"></div>
                        <div class="circle" id="circle2"></div>
                        <div class="circle" id="circle3"></div>
                    </div>
                
                    <button id="replayButton">New Trial</button>
                
                    <div id="buttons">
                        <button id="btn1">Circle 1</button>
                        <button id="btn2">Circle 2</button>
                        <button id="btn3">Circle 3</button>
                    </div>
                
                    <div id="result"></div>
                    
                    <p> Here's a demo to give a sense of what the experiment was like. Disclaimer! Just like in the color-matching demo, this is NOT the actual test. We can't perform the test for tetrachromacy using normal display monitors because they only have three types of phosphors.</p>

                    <p>In this <a href = "https://jov.arvojournals.org/article.aspx?articleid=2191517&fbclid=IwAR0CAFPh69vVRaHpwybsCUfZg144foBu_GGTcjEMOdLvB-iAPJTFScAJkSw">Journal of Vision paper from 2010</a>, Jordan and colleagues found that only one of the twenty four obligate carriers they studied was actually able to discriminate between lights that are totally identical to trichromats. Below is a plot of the mean errors in the Rayleigh Discrimination task as a function of mixture ratio. Error rates increased for intermediate ratios for most participants. But see the open circles -- subject cDa29 -- they had no trouble doing this task which stumped the rest of them.</p>
                    <p><img src="images/tetrachromat_data.png" style="width:700px;" alt = 'Data from Tetrachromacy test study'></p>

                    <p>In this case, the knowledge of biology, that the properties of our cones constrain our perception and that a subset of females who are mothers of anamalous trichromats might have four cones tuned to specific wavelengths, informed who to study and what to look for in the behavior. So we&#39;ve come full circle, from behavior predicting biology to biology predicting behavior. </p>
                    <!-- <p>I find the story of color science inspirational.  It&#39;s a point in support of the crucial role of <a href="Yael Niv Primacy of Behavioral Research">behavioral research in neuroscience</a>. It's also fascinating to see a scientific story play out across centuries.  </p> -->
                    <hr>
                    <p>Most of what I wrote about here has been previously explained by others. In particular, I recommend checking out: </p>
                    <ul>
                    <li><a href = "https://foundationsofvision.stanford.edu/chapter-4-wavelength-encoding/">Foundations of vision by Brian Wandell (chapter 4)</a></li>
                    <li><a href = "https://edyong.me/an-immense-world"> Ed Yong&#39;s An Immense World (chapter on color: &quot;Yurple, Rurple, Gurple&quot;)</a></li>
                    <li><a href = "https://www.youtube.com/watch?v=eKKXJyabCAQ">Eero Simoncelli&#39;s lecture on probing sensory representations </a> </li>
                    
                    </ul>
                    <p> Thanks to Rithika Sankar for patiently explaining basic genetics to me.</p>
                    <p> Please <a href="mailto:adithyanarayan101@gmail.com">let me know</a> if you spot any errors or mistakes. I'd like to be accurate but I'm still learning, so I greatly appreciate any feedback. </p>
                    <hr>

                </article>
            </div>

            
        </div>
    </main>
    
    <script>
        // let randomCircleIndex = null; // This will store which circle has the random color
        // let randomColor = null; // This will store the RGB of the random color

        // Function to generate a random color between red and green (including full red, full green)
        function generateRandomColor() {
            const red = Math.floor(Math.random() * 6)*10+98; // Random value for red (0 to 255)
            const green = 255-red; // Random value for green (0 to 255)
            return { r: red, g: green }; // Return an object with red and green values
        }

        // Function to calculate the ratio R / (R + G) for the random color
        function calculateRatio(randomColor) {
            const r = randomColor.r;
            const g = randomColor.g;
            // Calculate the ratio of red to the sum of red and green, avoiding division by zero
            const ratio = (r + g) === 0 ? 0 : r / (r + g);
            return ratio.toFixed(2); // Return the ratio rounded to 2 decimal places
        }

        // Function to set the colors of the circles
        function setCircleColors() {
            const circles = document.querySelectorAll('.circle');
            
            // Set two circles with 50% red and 50% green
            const redGreen = "rgb(128, 128, 0)"; // 50% Red + 50% Green
            
            // Set one circle with a random mixture of red and green
            randomColor = generateRandomColor();
            
            // Create an array of circle colors (the random color will be converted to rgb format)
            const colors = [redGreen, redGreen, `rgb(${randomColor.r}, ${randomColor.g}, 0)`];

            // Shuffle the colors array to randomize the order
            for (let i = colors.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [colors[i], colors[j]] = [colors[j], colors[i]]; // Swap elements
            }
            
            // Assign the shuffled colors to the circles and store the random circle index
            circles.forEach((circle, index) => {
                circle.style.backgroundColor = colors[index];
            });

            // Store the index of the random circle (the one with the random color)
            randomCircleIndex = colors.indexOf(`rgb(${randomColor.r}, ${randomColor.g}, 0)`);
        }

        // Function to show each circle with a blank in between
        function showCirclesWithBlank() {
            const circles = document.querySelectorAll('.circle');
            let delay = 0;
            const displayTime = 500;  // Time to display each circle (ms)
            const blankTime = 500;    // Time to show blank between circles (ms)

            circles.forEach((circle, index) => {
                // Show circle after delay
                setTimeout(() => {
                    circle.style.display = 'block';  // Make the circle visible
                }, delay);

                // Hide the circle after display time to simulate the "blank" screen
                setTimeout(() => {
                    circle.style.display = 'none';  // Hide the circle again
                }, delay + displayTime); // Circle disappears after displayTime
                
                // Increment delay for the next circle
                delay += displayTime + blankTime;  // Display time + blank time
            });
        }

        // // Function to reset the circles and replay the animation
        function replayAnimation() {
            const circles = document.querySelectorAll('.circle');
            // First, hide all the circles
            circles.forEach(circle => {
                circle.style.display = 'none';
            });
            // Set new colors and start the animation again
            setCircleColors();  
            showCirclesWithBlank(); 

            // Reset result text and enable answer buttons
            document.getElementById('result').textContent = '';
            enableAnswerButtons();
        }

        // // Function to check the user's choice
        function checkAnswer(choice) {
            const result = document.getElementById('result');
            const buttons = document.querySelectorAll('#buttons button');

            // Calculate the ratio of R / (R + G) for the random color
            const ratio = calculateRatio(randomColor);

            // Display whether the answer is correct or not, along with the ratio
            if (choice === randomCircleIndex) {
                result.textContent = `Correct! The ratio of R / (R + G) for the random color is: ${ratio}.`;
            } else {
                result.textContent = `Wrong! The ratio of R / (R + G) for the random color is: ${ratio}.`;
            }

            // Disable all answer buttons after the user makes a choice
            disableAnswerButtons();
        }

        // // Enable answer buttons after the animation is displayed
        function enableAnswerButtons() {
            const buttons = document.querySelectorAll('#buttons button');
            buttons.forEach(button => button.disabled = false);
        }

        // Disable answer buttons after the user selects an answer
        function disableAnswerButtons() {
            const buttons = document.querySelectorAll('#buttons button');
            buttons.forEach(button => button.disabled = true);
        }

        // Set the colors and start the animation when the page loads
        window.onload = () => {
            setCircleColors();  // Set initial colors
            showCirclesWithBlank();  // Show circles with blank in between
            enableAnswerButtons();  // Enable the answer buttons
        };

        // Add event listener for the replay button
        document.getElementById('replayButton').addEventListener('click', replayAnimation);

        // Add event listeners for the answer buttons
        document.getElementById('btn1').addEventListener('click', () => checkAnswer(0));
        document.getElementById('btn2').addEventListener('click', () => checkAnswer(1));
        document.getElementById('btn3').addEventListener('click', () => checkAnswer(2));


        const redSlider = document.getElementById('red');
        const greenSlider = document.getElementById('green');
        const blueSlider = document.getElementById('blue');
        const leftSemicircle = document.getElementById('leftSemicircle');
        const rightSemicircle = document.getElementById('rightSemicircle');
        const redValue = document.getElementById('redValue');
        const greenValue = document.getElementById('greenValue');
        const blueValue = document.getElementById('blueValue');
        const hexValue = document.getElementById('hexValue');
        const resetButton = document.getElementById('resetButton');
        const randomizeButton = document.getElementById('randomizeButton');

        // Function to generate a random color
        function randomColorSemi() {
            const r = Math.floor(Math.random() * 256);
            const g = Math.floor(Math.random() * 256);
            const b = Math.floor(Math.random() * 256);
            return `rgb(${r}, ${g}, ${b})`;
        }

        // Set a random color to the left semicircle
        leftSemicircle.style.backgroundColor = randomColorSemi();

        function updateColor() {
            const r = redSlider.value;
            const g = greenSlider.value;
            const b = blueSlider.value;

            rightSemicircle.style.backgroundColor = `rgb(${r}, ${g}, ${b})`;

            redValue.textContent = r;
            greenValue.textContent = g;
            blueValue.textContent = b;

            const hex = ((1 << 24) + (r << 16) + (g << 8) + b).toString(16).slice(1).toUpperCase();
            hexValue.textContent = `Hex: #${hex}`;
        }

        function randomizeTopColor() {
            leftSemicircle.style.backgroundColor = randomColorSemi();
        }

        redSlider.addEventListener('input', updateColor);
        greenSlider.addEventListener('input', updateColor);
        blueSlider.addEventListener('input', updateColor);

        randomizeButton.addEventListener('click', randomizeTopColor); // Add event listener for randomizing
        resetButton.addEventListener('click', () => {
            redSlider.value = 127;
            greenSlider.value = 127;
            blueSlider.value = 127;
            updateColor();
        });

        // Initialize color on load
        updateColor();
    </script>


</body>
</html>
