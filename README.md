<html>
<head>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<link rel="shortcut icon" href="images/icon.ico">
<style type="text/css">
	body {
		background-color: #f5f9ff;
		font-family: Arial, sans-serif;
		line-height: 2;
		font-size: 20px;
	}

	/* Hide both math displays initially, will display based on JS detection */
  .mathjax-mobile, .mathml-non-mobile { display: none; }

  /* Show the MathML content by default on non-mobile devices */
  .show-mathml .mathml-non-mobile { display: block; }
  .show-mathjax .mathjax-mobile { display: block; }

	.content-margin-container {
		display: flex;
		width: 100%; /* Ensure the container is full width */
		justify-content: left; /* Horizontally centers the children in the container */
		align-items: center;  /* Vertically centers the children in the container */
	}
	.main-content-block {
		width: 70%; /* Change this percentage as needed */
    max-width: 1100px; /* Optional: Maximum width */
		background-color: #fff;
		border-left: 1px solid #DDD;
		border-right: 1px solid #DDD;
		padding: 8px 8px 8px 8px;
		font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;#"Avenir";
	}
	.margin-left-block {
			font-size: 14px;
			width: 15%; /* Change this percentage as needed */
			max-width: 130px; /* Optional: Maximum width */
			position: relative;
			margin-left: 10px;
			text-align: left;
			font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;#"Avenir";
			padding: 5px;
	}
	.margin-right-block {
			font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;#"Avenir";
			font-size: 14px;
			width: 25%; /* Change this percentage as needed */
			max-width: 256px; /* Optional: Maximum width */
			position: relative;
			text-align: left;
			padding: 10px;  /* Optional: Adds padding inside the caption */
	}

	img {
			max-width: 100%; /* Make sure it fits inside the container */
			height: auto;
			display: block;
			margin: auto;
	}
	.my-video {
			max-width: 100%; /* Make sure it fits inside the container */
			height: auto;
			display: block;
			margin: auto;
	}
	/* Hide both video displays initially, will display based on JS detection */
  .vid-mobile, .vid-non-mobile { display: none; }

  /* Show the video content by default on non-mobile devices */
  .show-vid-mobile .vid-mobile { display: block; }
  .show-vid-non-mobile .vid-non-mobile { display: block; }

	a:link,a:visited
	{
		color: #0e7862; /*#1367a7;*/
		text-decoration: none;
	}
	a:hover {
		color: #24b597; /*#208799;*/
	}

	h1 {
		font-size: 18px;
		margin-top: 4px;
		margin-bottom: 10px;
	}

	table.header {
    font-weight: 300;
    font-size: 17px;
    flex-grow: 1;
		width: 70%;
    max-width: calc(100% - 290px); /* Adjust according to the width of .paper-code-tab */
	}
	table td, table td * {
	    vertical-align: middle;
	    position: relative;
	}
	table.paper-code-tab {
	    flex-shrink: 0;
	    margin-left: 8px;
	    margin-top: 8px;
	    padding: 0px 0px 0px 8px;
	    width: 290px;
	    height: 150px;
	}

	.layered-paper { /* modified from: http://css-tricks.com/snippets/css/layered-paper/ */
		box-shadow:
		        0px 0px 1px 1px rgba(0,0,0,0.35), /* The top layer shadow */
		        5px 5px 0 0px #fff, /* The second layer */
		        5px 5px 1px 1px rgba(0,0,0,0.35), /* The second layer shadow */
		        10px 10px 0 0px #fff, /* The third layer */
		        10px 10px 1px 1px rgba(0,0,0,0.35); /* The third layer shadow */
		margin-top: 5px;
		margin-left: 10px;
		margin-right: 30px;
		margin-bottom: 5px;
	}

	hr {
    height: 1px; /* Sets the height of the line to 1 pixel */
    border: none; /* Removes the default border */
    background-color: #DDD; /* Sets the line color to black */
  }

	div.hypothesis {
		width: 80%;
		background-color: #EEE;
		border: 1px solid black;
		border-radius: 10px;
		-moz-border-radius: 10px;
		-webkit-border-radius: 10px;
		font-family: Courier;
		font-size: 18px;
		text-align: center;
		margin: auto;
		padding: 16px 16px 16px 16px;
	}

	div.citation {
    font-size: 0.8em;
    background-color:#fff;
    padding: 10px;
		height: 200px;
  }

	.fade-in-inline {
		position: absolute;
		text-align: center;
		margin: auto;
		-webkit-mask-image: linear-gradient(to right,
																			transparent 0%,
																			transparent 40%,
																			black 50%,
																			black 90%,
																			transparent 100%);
		mask-image: linear-gradient(to right,
																transparent 0%,
																transparent 40%,
																black 50%,
																black 90%,
																transparent 100%);
		-webkit-mask-size: 8000% 100%;
		mask-size: 8000% 100%;
		animation-name: sweepMask;
		animation-duration: 4s;
		animation-iteration-count: infinite;
		animation-timing-function: linear;
		animation-delay: -1s;
	}

	.fade-in2-inline {
			animation-delay: 1s;
	}

	.inline-div {
			position: relative;
	    display: inline-block; /* Makes both the div and paragraph inline-block elements */
	    vertical-align: top; /* Aligns them at the top, you can adjust this to middle, bottom, etc., based on your needs */
	    width: 50px; /* Optional: Adds space between the div and the paragraph */
	}

</style>

	  <title>The Platonic Representation Hypothesis</title>
      <meta property="og:title" content="The Platonic Representation Hypothesis" />
			<meta charset="UTF-8">
  </head>

  <body>

		<div class="content-margin-container">
				<div class="margin-left-block">
				</div>
		    <div class="main-content-block">
						<table class="header" align=left>
								<tr>
									<td colspan=4>
										<span style="font-size: 32px; font-family: 'Courier New', Courier, monospace; /* Adds fallbacks */">Foundations of Interpretability: Expanding the Toy Model Framework</span>
									</td>
								</tr>
								<tr>
										<td align=left>
												<span style="font-size:17px"><a href="blog_template/your_website">Joseph Atie</a></span>
										</td>
										<td align=left>
												<span style="font-size:17px"><a href="blog_template/your_partner's_website">Abhilash Rao</a></span>
										</td>
										<td align=left>
											<span style="font-size:17px"><a href="blog_template/your_partner's_website">Arthur Pommersheim</a></span>
									</td>
								<tr>
									<td colspan=4 align=left><span style="font-size:18px">Final project for 6.7960, MIT</span></td>
								</tr>
						</table>
					</div>
					<div class="margin-right-block">
					</div>
		</div>

		<div class="content-margin-container" id="intro">
				<div class="margin-left-block">
          <!-- table of contents here -->
          <div style="position:fixed; max-width:inherit; top:max(20%,120px)">
              <b style="font-size:16px">Outline</b><br><br>
              <a href="#intro">Introduction</a><br><br>
              <a href="#does_x_do_y">Does X do Y?</a><br><br>
              <a href="#implications_and_limitations">Implications and limitations</a><br><br>
          </div>
				</div>
		    <div class="main-content-block">
            <!--You can embed an image like this:-->
            
		    </div>
		</div>

    <div class="content-margin-container" id="intro">
			<div class="margin-left-block">
			</div>
		    <div class="main-content-block">
						<h2>Introduction</h2>
						<p>
						In the ever-expanding domain of deep learning, the ability of neural networks to process and represent high-dimensional data efficiently 
						remains one of their most remarkable yet least understood capabilities. A key aspect of this efficiency lies in dimensionality reduction, 
						where networks compress vast amounts of information into lower-dimensional embeddings while retaining meaningful features. This process is 
						central to the power of deep learning, enabling models to generalize, reduce noise, and efficiently handle the curse of dimensionality.
						</p>
						<p>
						However, despite its importance, dimensionality reduction often acts as a "black box" and make neural network less interpretable. Wouldn't it have 
						been nicer if each neuron in the neural network represented only one feature? For example, in the context of CNNs, it would be more 
						intuitive if one neuron were solely responsible for detecting curvature, while another solely focused on detecting color. Unfortunately the reality 
						is different. When a network creates a compact embedding, each feature meets one of three fates: </p>
						<p>
						(1) The feature is exclusively encoded by a single dedicated monosementic neuron. <br>
						(2) The feature is jointly encoded by a polysementic neuron alongside another feature (superposition). <br>
						(3) The feature is ignored by the model.
						</p>
						<p>
						It is specifically the phenomenon observed in (2)—polysemantic encoding—that makes neural networks less interpretable. To build intuition around 
						this, recent work such as [Paper X] and [Paper Y] has begun to uncover the mechanism of superposition. These studies use ReLU networks to investigate 
						how a neural network decides to encode an input feature based on factors like feature importance and sparsity.
						</p>
						<p>
						<b>The gap this project aims to fill</b><br>
						While these studies provide an important first step toward building intuition about encoding mechanisms, they leave critical practical questions unanswered. For instance, how do choices in network 
						architecture, such as activation functions or the number of hidden dimensions, impact the emergence and stability of superposition? What conditions 
						are required for superposition to succeed without introducing noise or degrading model performance? <br><br>
						Our project aims to address these questions by systematically exploring the dynamics of superposition within simplified toy models. Using these 
						interpretable frameworks, we will experiment with altering key factors, such as activation functions, optimizers, and network configurations, to 
						observe their effects on feature representation. These experiments are scientifically significant because they probe fundamental aspects of 
						representation learning that are critical to understanding how neural networks encode and compress information. While dimensionality reduction 
						has been extensively studied in larger models, the direct effects of architectural and training choices on superposition remain largely unexplored, 
						particularly in controlled, interpretable environments like toy models.
						</p>
						<p>
						<b>List of experiments</b><br>
						</p>
						<p>
						<b>Importance of this work</b><br>
						Our project advances theoretical understanding and provides actionable insights into designing more efficient and interpretable neural 
						networks, making it a valuable addition to the growing body of research in this area.
						</p>

		    </div>
		</div>

		<div class="content-margin-container" id="definitions">
			<div class="margin-left-block">
			</div>
		    <div class="main-content-block">
					<h2>Terminology and Definitions</h2>
					Before presenting our experimental results, we will define essential terminology to establish a common conceptual framework and ensure clarity throughout this study.
						<p><b>Features</b><br>
							The interpretation of what constitutes a feature varies across studies and applications. 
							In this study, we define features as input qualities that help differentiate one input from another. 
							Features can sometimes be directly observable, such as curvature or color in an image. 
							At other times, they may be conceptual and interpretable by humans, as demonstrated by the famous work 
							of Mikolov et al. [11], which showed that word embeddings can have directions corresponding to semantic 
							properties. This allows for operations like embedding arithmetic, exemplified by:
						</p>
						<blockquote>
							V("king") − V("man") + V("woman") = V("queen")
						</blockquote>
						<p>
							However, some features defy human understanding. Should this surprise us? It did—until we were inspired by the insights of Richard Hamming and Brett Victor in
							<i>The Unreasonable Effectiveness of Mathematics</i> and <i>Media for Thinking the Unthinkable</i>. Their perspectives help explain why certain concepts remain 
							elusive and how new frameworks can expand our comprehension:
						</p>
						<blockquote>
							"Just as there are odors that dogs can smell and we cannot, as well as sounds that dogs can hear and 
							we cannot, so too there are wavelengths of light we cannot see and flavors we cannot taste.
							Why then, given our brains wired the way they are, does the remark 'Perhaps there are thoughts we 
							cannot think,' surprise you?"
							<cite>- Richard Hamming, <i>The Unreasonable Effectiveness of Mathematics</i></cite>
						</blockquote>
						<blockquote>
							"These sounds that we can't hear, this light that we can't see, how do we even know about these things 
							in the first place? Well, we built tools. We built tools that adapt these things that are outside of 
							our senses, to our human bodies, our human senses. 
							We can't hear ultrasonic sound, but you hook a microphone up to an oscilloscope and there it is. 
							You're seeing that sound with your plain old monkey eyes. We can't see cells and we can't see galaxies, 
							but we build microscopes and telescopes and these tools adapt the world to our human bodies, to our 
							human senses. <br><br>
							When Hamming says there could be unthinkable thoughts, we have to take that as 'Yes, but we build 
							tools [neural networks] that adapt these unthinkable thoughts to the way that our minds work and 
							allow us to think these thoughts that were previously unthinkable."
							<cite>- Brett Victor, <i>Media for Thinking the Unthinkable</i></cite>
						</blockquote>

					</p>

					<p><b>Superposition</b><br>
					Imagine you're at a packed movie theater, but instead of seats, you have a limited number of beanbags. Each beanbag 
					can be shared by multiple people, as long as they squeeze in carefully and don’t completely overlap. Somehow, everyone 
					manages to sit comfortably, even though the number of beanbags seems too small for the crowd. This is superposition in action. </p>
					<p>
					In neural network, superposition is a clever strategy allowing neural networks "to represent more features than they have neurons"[add link]. 
					They exploit a property of high-dimensional spaces to simulate a model with many more neurons. 
					</p>

					<p><b>Sparsity</b><br>
					Feature Sparsity is a concept rooted in the observation that, in the natural world, many features are sparse—they occur only occasionally. For example, most parts of an image don’t 
					contain specific objects like a horizontal edge or a dog head, and most tokens in language don’t refer to rare concepts like "Martin Luther King" or "music." This idea builds on 
					classical work in vision and natural image statistics, where sparsity helps models focus only on the most relevant features at any given time. <br>
					In the toy model, feature sparsity is modeled using the probability <em>S</em>, which determines how often a feature in the 
					input vector is inactive (set to 0). Specifically:
					</p>
						<ul>
							<li>For a given dimension <em>x<sub>i</sub></em>, the feature is set to 0 with probability <em>S<sub>i</sub></em>, meaning it is inactive most of the time if <em>S<sub>i</sub></em> is high.</li>
							<li>Otherwise, with probability <em>1 - S<sub>i</sub></em>, the feature is active and takes a value uniformly distributed between 0 and 1.</li>
						</ul>
						<p>
							In practice, the toy model we're analyzing in this blog post assumes all features have the same sparsity <em>S</em>, meaning that all features share the same probability of being inactive. This sparse 
							distribution reflects real-world data structures, where only a subset of features is typically relevant at any given time.
						</p>
					<p>
						To gain a deeper understanding of the concept of sparsity, we modified the toy model to generate three distinct batches with varying levels of feature sparsity:
					</p>
						<ul>
							<li><strong>S = 0:</strong> Features are never set to 0 (all features are active).</li>
							<li><strong>S = 0.5:</strong> Features are set to 0 with a probability of 0.5, resulting in approximately half of the features being inactive.</li>
							<li><strong>S = 0.9:</strong> Features are set to 0 with a probability of 0.9, making most features inactive.</li>
						</ul>
					<p>
						The figures below illustrate the outputs for these different levels of sparsity, providing insights into how feature activation changes as the sparsity increases.
					</p>					
					<div class="image-container">
						<div class="image-caption"><strong>Figure 1: Output with S = 0 (All features active)</strong></div>
						<img src="images/sparsity0.png" alt="Sparsity with S=0">
					</div>
					<div class="image-container">
						<div class="image-caption"><strong>Figure 2: Output with S = 0.5 (Approximately half features active)</strong></div>
						<img src="images/sparsity05.png" alt="Sparsity with S=0.5">
					</div>
					<div class="image-container">
						<div class="image-caption"><strong>Figure 3: Output with S = 0.9 (Most features inactive)</strong></div>
						<img src="images/sparsity09.png" alt="Sparsity with S=0.9">
					</div>

					<p><b>Feature Importance</b><br>
					Imagine packing a suitcase for a trip where certain items, like your passport or medicine, are far more critical than others, such as an extra pair of shoes. 
					Naturally, you would prioritize these essential items to avoid serious consequences later. <br>
					Similarly, in the toy model, not all features are treated equally—some are far more important than others. In the toy model, feature importance assigns weights 
					<em>I<sub>i</sub></em> to each feature, reflecting its significance in the overall reconstruction. When the model makes predictions, the reconstruction error for each feature is scaled 
					by its importance. This means that disregarding or poorly reconstructing a highly important feature incurs a much higher cost than for a less important one. 
					The model is incentivized to focus its representational capacity on preserving more important features, ensuring that key patterns in the data are retained while 
					less critical ones can be approximated or ignored.
					</p>

					<p><b>Add additional terms as needed</b><br>
					</p>
					
		    </div>
		   
		</div>

		<div class="content-margin-container" id="currentwork">
			<div class="margin-left-block">
			</div>
		    <div class="main-content-block">
					<h2>The Model to Demonstrate Superposition</h2>
					<p>
						The experiment setup in this section creates a simplified environment to analyze how neural networks encode and reconstruct information when their capacity is limited.
					</p>
					<ul>
						<li>
							<strong>Input Features:</strong> The input consists of vectors (<em>x</em>) of fixed size <em>n</em>, with <em>n</em> features, where each feature is represented by a scalar value.
						</li>
						<li>
							<strong>Feature Sparsity:</strong> Features are not always active. A sparsity parameter (<em>S</em>) determines the probability that a feature is set to 0.
						</li>
						<li>
							<strong>Feature Importance Weights:</strong> Each feature has an associated importance value (<em>I</em>), influencing its contribution to the loss function. Higher importance features incur a greater penalty if not accurately reconstructed.
						</li>
						<li>
							<strong>Encoding and Decoding:</strong> The model uses a limited number of hidden units <em>m</em> (less than the total number of features, <em>m < n</em>) to encode the input, creating a bottleneck. The decoder then attempts to reconstruct the input features from this compressed representation.
						</li>
						<li>
							<strong>Reconstruction Error:</strong> The error for each feature is computed as the squared difference between the original and reconstructed values. This error is weighted by the feature's importance, prioritizing accurate reconstruction of important features.
						</li>
						<li>
							<strong>Optimization:</strong> The model is trained to minimize the total weighted reconstruction error, encouraging efficient use of its limited capacity while focusing on high-importance features.
						</li>
					</ul>
					<div class="image-container">
						<div class="image-caption"><strong>Figure 4: Network Architecture</strong></div>
						<img src="images/network_architecture.png" alt="Network Architecture">
					</div>
					<p>The toy model developed by [XX] employs the ReLU activation function to investigate how neural networks decide to encode each feature. This simplified approach helps uncover the fundamental mechanisms of feature representation. As we progress through this blog, we'll delve into various 
						activation functions and examine how they influence the encoding strategies of neural networks, highlighting their impact on our findings.</p>
					<div>
						<div class="title">Loss Function: </div>
						<div class="equation">
							\( L = \sum_{x} \sum_{i} I_i (x_i - x_i')^2 \)
						</div>
					</div>
					<br>
					<div class="title">ReLU Output Model Equations:</div>
						<div class="equation">
							\( h = Wx \)
						</div>
						<div class="equation">
							\( x' = \text{ReLU}(W^T h + b) \)
						</div>
						<div class="equation">
							\( x' = \text{ReLU}(W^T Wx + b) \)
						</div>
		    		</div>
		</div>

		<div class="content-margin-container">
				<div class="margin-left-block">
				</div>
		    <div class="main-content-block">
            <h2>Basic Results</h2>
            
						
		    </div>

		</div>

		<div class="content-margin-container">
				<div class="margin-left-block">
				</div>
			<div class="main-content-block">
			<h2>Experiment 1: Altering Activation Functions</h2>

			</div>
					
		</div>

		<div class="content-margin-container">
				<div class="margin-left-block">
				</div>
			<div class="main-content-block">
			<h2>Experiment 2: Altering Feature Importance</h2>
				<p>
					A simple way to understand which features the network is representing is by examining the matrix \( W^T W \), which has dimensions \( n \times n \), 
					where \( n \) is the number of features in the input vector. This matrix encodes how the network uses its embedding space to represent the input features.
					The diagonal elements, located at \( (i, i) \), indicate whether feature \( i \) is being represented by the network. 
				</p>
				<p>
					In this section, we aim to isolate the effect of feature importance on a neural network's decision to encode features. 
					To achieve this, we set the feature sparsity to \( S = 0 \) without modifying it, meaning the input vector is very dense. With this setup, the neural network determines which features to encode or 
					ignore based solely on their importance values. The activation function used in this experiment is ReLU. This approach allows us to examine how the model 
					allocates its representational capacity when feature sparsity is not a factor, providing a clearer understanding of the role of importance in feature selection.
				</p>
				<h1>Test Case 1: Features are ordered from more important to less important</h1>
				<p>
				In this test case, the input features are ordered by importance, starting with the most important and decreasing to the least important. 
				The importance values follow an exponential decay, with the most critical features receiving significantly higher weights than the less important ones.
				</p>
				<p>
					Model Configuration:
					<ul class="config-list">
						<li>Total number of features \(n\): 20</li>
						<li>Embedding size \(m\): 5</li>
						<li>Features Importance: Follows exponential decay</li>
						<li>Activation function: ReLU</li>
						<li>Input vector sparsity \(S\): 0</li>
					</ul>
				</p>
				<p>
					Results:
				</p>
				<p>
					In Figure 5, the left plot represents the L2 norms of the weight vectors corresponding to each feature. Each bar indicates the magnitude of a feature's contribution to the embedding space, 
					with taller bars reflecting stronger representation. In this case, the plot shows that the network focuses exclusively on a subset of features, as only the first five features have non-zero norms. 
					These features are represented uniformly, with no significant variations in their norms, suggesting equal prioritization. The absence of bars for the remaining features indicates that these features 
					have been completely disregarded by the network due to capacity constraints in the embedding space.
				</p>
				<p>
					The right plot is a heatmap showing the pairwise interference between features, computed as the dot 
					product of their weight vectors \(W^T W\). Each cell in the heatmap corresponds to the interaction between two features, with 
					brighter colors (red) indicating stronger interference. In this case, the heatmap reveals that the network's 
					embedding is highly orthogonal, as all off-diagonal elements are neutral (gray), indicating minimal overlap between 
					features. The strong diagonal elements confirm that each feature is primarily self-represented, with little to no 
					interference between different features.
				</p>
				<p>
					As our standard intuitions would expect, the model consistently selects the top-\( m \) most important features for the embedding. In our specific case, the model 
					selected the first 5 features—those with the highest importance—and ignored all remaining features. The behavior of the bias vector \( b \) is also noteworthy. 
					For the features selected to pass through the embedding, the corresponding entries in \( b \) are set to zero. For all other features, \( b \) contains the expected 
					value of the feature, ensuring that disregarded features do not contribute to the model's output.
					<div class="image-container">
						<div class="image-caption">Figure 5: Test Case 1 Results</div>
						<img src="images/features_decay_importance.png" alt="Features by Importance">
					</div>
				</p>
				<h1>Test Case 2: All features are assigned equal importance</h1>
				<p>
				In this test case, the input features are assigned equal importance. The purpose of this test case is to evaluate how the neural network would select which features to represent 
				when all features are equally important and when there isn't enough neurons to represent all features.
				</p>
				<p>
					Model Configuration:
					<ul class="config-list">
						<li>Total number of features \(n\): 20</li>
						<li>Embedding size \(m\): 5</li>
						<li>Features Importance: Uniform across features</li>
						<li>Activation function: ReLU</li>
						<li>Input vector sparsity \(S\): 0</li>
					</ul>
				</p>
				<p>
					Results:
				</p>
				<p>
					When all features are assigned equal importance, the neural network distributes its representational capacity more evenly across the input features. This leads to a noticeable 
					increase in feature interference, as shown in the heatmap, where overlapping representations are more prevalent. Interestingly, despite equal importance, certain features still 
					exhibit slightly higher norms, suggesting that the network inherently favors specific features, possibly due to subtle biases in the initialization or training dynamics. This 
					result highlights the critical role of prioritization in reducing interference and efficiently utilizing limited embedding space. When feature importance is unequal, the network 
					can focus on the most critical features, minimizing overlap and improving separability, whereas equal importance forces the network to rely more heavily on superposition, potentially 
					compromising representational efficiency.
					<div class="image-container">
						<div class="image-caption">Figure 6: Test Case 2 Results</div>
						<img src="images/features_uniform_importance.png" alt="Features by Importance">
					</div>
				</p>
				<h1>Test Case 3: Clustered Importance</h1>
				<p>
					In this clustered importance test case, we assign distinct importance levels to groups of input features, creating high- and low-priority clusters.
				</p>
				<p>
					Model Configuration:
					<ul class="config-list">
						<li>Total number of features \(n\): 20</li>
						<li>Embedding size \(m\): 5</li>
						<li>Features Importance: [1, 1, 1, 1, 1, 0.5, 0.5, 0.5, 0.5, 0.5]</li>
						<li>Activation function: ReLU</li>
						<li>Input vector sparsity \(S\): 0</li>
					</ul>
				</p>
				<p>
					Results:
				</p>
				<p>
					The clustered importance experiment reveals surprising behavior in how neural networks allocate their representational capacity. Despite assigning equal importance to the first five features, 
					the model selectively represents only three of them, while the other two are deprioritized. This indicates that the network does not strictly follow the assigned importance weights but instead 
					considers other factors, such as redundancy among features or the ease of representing certain features in the reduced embedding space. Even more unexpectedly, some features with lower importance 
					(e.g., importance = 0.5) were represented more prominently than certain high-importance features (importance = 1.0). This suggests that lower-importance features might have been less complex or 
					more "compatible" with the embedding constraints, allowing the network to encode them more efficiently. Additionally, some features, regardless of their assigned importance, were completely dropped, 
					showing the network's ability to optimize capacity by focusing on features that are easier to represent or more useful for minimizing the loss. 
					<div class="image-container">
						<div class="image-caption">Figure 7: Test Case 3 Results</div>
						<img src="images/features_cluster_importance.png" alt="Features by Importance">
					</div>
				</p>
			</div>
		</div>

	</div>

		<div class="content-margin-container" id="implications_and_limitations">
				<div class="margin-left-block">
				</div>
		    <div class="main-content-block">
						<h1>Implications and limitations</h1>
						Let's end with some discussion of the implications and limitations.
		    </div>
		    <div class="margin-right-block">
		    </div>
		</div>

		<div class="content-margin-container" id="citations">
				<div class="margin-left-block">
				</div>
		    <div class="main-content-block">
						<div class='citation' id="references" style="height:auto"><br>
							<span style="font-size:16px">References:</span><br><br>
							<a id="ref_1"></a>[1] <a href="https://en.wikipedia.org/wiki/Allegory_of_the_cave">Allegory of the Cave</a>, Plato, c. 375 BC<br><br>
							<a id="ref_2"></a>[2] <a href="">A Human-Level AGI</a>, OpenAI, 2025<br><br>
						</div>
		    </div>
		    <div class="margin-right-block">
            <!-- margin notes for reference block here -->
		    </div>
		</div>

	</body>

</html>
