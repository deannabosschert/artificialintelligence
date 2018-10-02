# Artificial Intelligence
@Susanna S die spellingcheck komt vanuit Chrome, niet vanuit Dropbox Paper zelf. Heb er zelf net eindelijk Engels aan toegevoegd haha.

# Applications: NPC’s
- Short summary of A.I.

Artificial Intelligence: Artificial intelligence is a form of intelligence that does not have a           biological foundation, meaning its origin is of scientific and mathematic networks. Artificial intelligence – in advanced state – mimics parts of the human brain and is potentially capable of complex- problem solving, making interactions between other systems and human beings and making predictions.

- Definition of A.I. in games

Game A.I. is not the same as A.I. that is used academically. The A.I. in games is based on concrete details of the gaming environment, which is part of the subsystem, containing feature and schedule revision. The goal of A.I. in computer games is not to compute the most optimal behavior for winning against the player. Instead, the outcome should be as believable and fun as possible. 

- Examples of first usage + ‘simple’ usage (‘dumb’ AI's)

→ Pong, Chess, later usage in Tamagotchi


- Example of high-end usage (e.g. Skyrim)
- Future



# Literature (Deanna)

Ik gooi het gewoon in hetzelfde document haha mss heb jij er ook nog wat aan

## [Adam Geitgey (2016) - Machine learning is fun (Part 1)](https://moodle.cmd.hva.nl/mod/url/view.php?id=25043)

**What is machine learning?**
Machine learning is the idea that there are generic algorithms that can tell you something interesting about a set of data without you having to write any custom code specific to the problem. Instead of writing code, you feed data to the generic algorithm and it builds its own logic based on the data.

**Machine learning:** an umbrella term covering lots of kinds of generic algorithms.

**Classification algorithm:** can put data into different groups. Can be used for different purposes; it’s fed different training data so it comes up with different classification logic.


![This machine learning algorithm is a black box that can be re-used for lots of different classification problems.](https://cdn-images-1.medium.com/max/1000/1*YXiclXZdJQVJZ0tQHCv5zw.png)



## Two kinds of Machine Learning Algorithms:
****- Supervised learning
****- Unsupervised learning


## Supervised learning:

Using the training data to predict the prices of other [houses].
You knew the answer to the problem and could work backwards from there to figure out the logic.

![Oh no! A devious student erased the arithmetic symbols from the teacher’s answer key!](https://cdn-images-1.medium.com/max/1000/1*SihYXaJQS3T6tOwqJ6fzPw.png)


You are letting the computer work out that relationship for you. And once you know what math was required to solve this specific set of problems, you could answer to any other problem of the same type!





## Unsupervised learning:

What if you didn’t know the sale price for each [house]? 
This is kind of like someone giving you a list of numbers on a sheet of paper and saying “I don’t really know what these numbers mean but maybe you can figure out if there is a pattern or grouping or something — good luck!”


![Default data](https://cdn-images-1.medium.com/max/1000/1*mUJw2yL4-OBI25xUKS7_Bg.png)



What to do with this data? e.g.

- Automatically identify different market segments in your data.
- Automatically identify any outlier houses that were way different than everything else.

→ **Machine learning:** figuring out an equation to solve a specific problem based on some example data

*[for the mathemetic examples, check the URL]*

![](https://cdn-images-1.medium.com/max/800/1*LlTIwE6h0l1Aoln2GlAGcw.png)





## Facts
- Generic learning algorithms that “stir the number stew” out-perform approaches where real people try to come up with explicit rules themselves. The “dumb” approach of machine learning eventually beats human experts.
- All it knows is that it needs to stir in some amount of those numbers to get the correct answer.
- It’s very likely you’ll have no idea ***why*** a particular set of weights will work. 


## “Try every number” explained:


![Original equation](https://cdn-images-1.medium.com/max/1000/1*4j82aAIUGQKKUmKcHLMWJQ.png)


Rewritten:


![θ is what represents your current weights. J(θ) means the ‘cost for your current weights’.](https://cdn-images-1.medium.com/max/1000/1*ZyboMOVQ5zOv0ZTC4a3usA.png)


***E (sigma) uitgelegd:***
***for (i = 1; i <= m; i++) {*
    *// de inhoud*
*}*

If I’m not mistaken, in unsupervised machine learning, the machine will try out lots. Then, we compare those answers to the actual correct answers and calculate how much the machine is off (how wrong the [price] is for the correct answers).


![The graph of our cost function looks like a bowl. The vertical axis represents the cost.](https://cdn-images-1.medium.com/max/1000/1*prsH6EfJmFqdmFElj1Ht8g.png)


Blue: where the machine is the least wrong
Red: where the machine is the most wrong
The goal: getting the whole graph down to the blue zone!

[NL for clarity: De afgeleide functie is niets anders dan een functie die ogenblik die steilheid van de grafiek geeft, zonder zelfs de grafiek of de raaklijn maar te tekenen]

**Batch gradient descent: s**o if we calculate a partial derivative of our cost function with respect to each of our weights, then we can subtract that value from each weight. That will walk us one step closer to the bottom of the hill. Keep doing that and eventually we’ll reach the bottom of the hill and have the best possible values for our weights.


## Multivariate linear regression

You are estimating the equation for a line that fits through all of your house data points. Then you are using that equation to guess the sales price of houses you’ve never seen before based where that house would appear on your line. 

**Overfitting:** it’s easy to come up with a set of weights that always works perfectly for predicting the prices of the houses in your original data set but never actually works for any new houses that weren’t in your original data set. There are ways to deal with this, though.

Machine Learning in a nutshell:
Just feed in the data and watch the computer magically figure out the equation that fits the data!


![There isn’t any kind of relationship between the potted plants in each house and the home’s sale price](https://cdn-images-1.medium.com/max/1000/1*N6pxRoVoEoedFELL2HdxbA.png)




***Remember that machine learning only works if the problem is actually solvable with the data that you have.***





## [Adam Geitgey (2016) - Machine learning is fun (Part 2)(optional)](https://medium.com/@ageitgey/machine-learning-is-fun-part-2-a26a10b68df3)

(deze is niet verplicht maar muh autism kan het niet aan dat ie er tussenuit wordt gelaten)

This was the original code, represented in a simple diagram: 

![](https://cdn-images-1.medium.com/max/1000/1*LlTIwE6h0l1Aoln2GlAGcw.png)


This algorithm only works for simple problems where the result has a *linear* relationship with the input. What if the truth behind house prices isn’t so simple? Maybe the neighborhood matters a lot for big houses and small houses but doesn’t matter at all for medium-sized houses. 



What if we run this algorithm multiple times with different of weights that each capture different edge cases? :

![](https://cdn-images-1.medium.com/max/1000/1*hOemQF_v42KHlMyiqcQNyQ.png)


Then, we combine those final price estimates into another diagram:

![](https://cdn-images-1.medium.com/max/1000/1*VeS0ziSjogCQThPYZh0TIQ.png)


Of course, this diagram refers back the the former diagrams. 









So, the final diagram to capture all would be:

![](https://cdn-images-1.medium.com/max/1000/1*Lt8RZaeQ6f6B_eA1oD32JQ.png)


Whoop whoop! This is called the **Neural Network.** Every circle is a *node/neuron*, now chained together. Each one contains a simple function. so we can model functions that are too complicated to be modeled by one single neuron.


## Memory

**Stateless algorithm**: without memory. It cannot respond to patterns in data over time.

Example: guess the first letter someone is going to type.
Neurons used: English language, past stories written, common letter to begin a word with etc


![](https://cdn-images-1.medium.com/max/1000/1*e2YPupJVOiZj4B_nGZi5pQ.png)


**Adding state to our model:** each time we ask our neural network for an answer, we also save a set of our intermediate calculations and re-use them the next time as part of our input

**Recurrent** ********Neural Network:** updating the network each time we use it, so it’ll update its predictions based on what it saw most recently. Can even model patterns over time.

***As machine learning becomes more important in more industries, the difference between a good program and a bad program will be how much data you have to train your models. That’s why companies like Google and Facebook need your data so badly!***

## [Adam Geitgey (2016) - Machine learning is fun (Part 3)](https://moodle.cmd.hva.nl/mod/url/view.php?id=25060)

Example: try to recognize the number ’8’ from photo's of handwriting
Data: 60,000 images of handwritten digits

Just think about it: a neural network takes numbers as input. To a computer, an image is really just a grid of numbers that represent how dark each pixel is. Below 8’s just an array of 18*18 pixels.


![](https://cdn-images-1.medium.com/max/1250/1*UDgDe_-GMs4QQbT8UopoGA.png)


So, just enlarge our amount of nodes to 324! (18*18..)

![](https://cdn-images-1.medium.com/max/1000/1*b31hqXiBUjIXo2HSn_grFw.png)


What’s up next?:
Classify the objects into groups and train the neural network with images of “8”s and not-“8"s so it learns to tell them apart. Boom!


## Tunnel vision

Flaw: above will only work when the letter is perfectly centered each time.

![Perfectly centered](https://cdn-images-1.medium.com/max/1000/1*5ciREAL7xdyXcD-cSRP7Jw.png)

![Not so perfectly centered](https://cdn-images-1.medium.com/max/1000/1*b5jMTAiyVhOIB9hheXhMmA.png)

## Possible solutions: 
- **Searching with a Sliding Window**
![Super inefficient.](https://cdn-images-1.medium.com/max/1000/1*bGBijVuJnTRj8025et0mcQ.gif)

- **More data and a Deep Neural Net**

Train the machine with more data! We can even write a script to generate more data.

![Synthetic Training Data: creating different versions of the training images we already had.](https://cdn-images-1.medium.com/max/1000/1*biD9eS5eB6zXzieonNk-VQ.png)


This will make the problem harder for our neural network to solve, but we can compensate for that by making our network bigger and thus able to learn more complicated patterns.

To make the network bigger, we just stack up layer upon layer of nodes:

![Deep neural network: because it has more layers than a traditional neural network.](https://cdn-images-1.medium.com/max/1000/1*wfmpsoFqWKC7VadjTJxwnQ.png)


Downside: this is very slow. Why would you treat each possibility as a different object?

## The Solution is Convolution

Right now, our machine doesn’t understand that moving an object around in the picture doesn’t make it something different. This means it has to re-learn the identify of each object in every possible position. 

**Translation invariance** **— an “8” is an “8” no matter where in the picture it shows up.
**Convolution:** instead of feeding entire images into our neural network as one grid of numbers, do something that takes advantage of the idea that an object is the same no matter where it appears in a picture

**Step 1: Break the image into overlapping image tiles**

![Similar to our sliding window search above, pass a sliding window over the entire original image and save each result as a separate, tiny picture tile. Total of 77 tiles.](https://cdn-images-1.medium.com/max/1000/1*xS7EugfgQHk68iph7GHpQg.png)


**Step 2: Feed each image tile into a small neural network**
We’ll keep the **same neural network weights** for every single tile in the same original image. Only when something interesting happens, it’ll mark the tile as such.

![Repeat this 77 times, once for each tile.](https://cdn-images-1.medium.com/max/1000/1*84-TdHvtAHkfnzwa1ZsTVg.png)


**Step 3: Save the results from each tile into a new array**
Save the result from processing each tile into a grid in the same arrangement as the original image

![Start with a large image and end with a slightly smaller array that records which sections were interesting.](https://cdn-images-1.medium.com/max/1000/1*tpMqyjAFgsYWpvlNkZgFfw.png)


**Step 4: Downsampling**
The previous array is still quite big. We gotta downsample that!

![We’ll just look at each 2x2 square of the array and keep the biggest number:](https://cdn-images-1.medium.com/max/1000/1*xOAroFiw9X0WSkCwgcIO6Q.png)


Keep the most interesting bit each time.

**Final step: Make a prediction**
So, we now got a smaller array. Let’s put that into another neural network! This final network will determine if it’s a match.


![From start to finish](https://cdn-images-1.medium.com/max/1000/1*tJ1Rkl5xw_5izEZXmNfh5Q.png)

![Above example but more realistic](https://cdn-images-1.medium.com/max/1000/1*JSnKtzEgiHd4p6UlNv_C7w.png)


***The more convolution steps you have, the more complicated features your network will be able to learn to recognize. It’s all trial and error to find the right combinations***

***In machine learning, having more data is almost always more important that having better algorithms.***


## Testing our Network

To really see how effective our network is, we need to test it with lots of images.
To judge how good a classification system really is, we need to look closely at *how* it failed, not just the percentage of the time that it failed.

**Predictions:**

- True positives: correctly identified as birds
- True negatives: correctly identified as “not a bird”
- False positives: thought were birds but were not really birds at all
- False negatives: didn’t correctly recognize as birds


![](https://cdn-images-1.medium.com/max/1000/1*lgSDQ4-Js3elXBpavIp6FA.png)


**Precision and Recall** metrics give us a clearer picture of how well we did:

![](https://cdn-images-1.medium.com/max/1000/1*T8SURWDvTTEY37yjUvu_pQ.png)




## [Artificial Intelligence and Life in 2030 (page 12 t/m 17)](https://moodle.cmd.hva.nl/mod/url/view.php?id=25059)

**SECTION I: WHAT IS ARTIFICIAL INTELLIGENCE?**

## Defining AI

There isn’t an universal accepted definition of AI, and this has helped the field to grow at a high pace. Instead, we are guided by a rough sense of direction.

***“Artificial intelligence is that activity devoted to making machines intelligent, and intelligence is that quality that enables an entity to function appropriately and with foresight in its environment.”***

From this perspective, the characterizing of AI depends on the credit one is willing to give this synthesized soft-and hardware for functioning ‘***appropriately and with foresight’.***
For example: would you consider a simple calculator intelligent?

The Study Panel finds: the difference between an arithmetic calculator and a human brain is not one of kind, but of:

- Scale
- Speed
- Degree of autonomy
- Generality

This will place every other instance of intelligence at some appropriate location in the spectrum.
The calculator will be placed somewhere within this spectrum, but cannot be compared with today’s AI’s.

**“AI effect” / “odd paradox”:**  people become accustomed to a new technology, it stops being considered AI and newer technologies will emerge.

I’d say this is quite ironical as AI does not “deliver” a life-changing product as a bolt from the blue. Rather, AI technologies continue to get better in a continual, incremental way


## The Human Measure

Notably, the characterization of intelligence as a spectrum grants no special status to the human brain. Then again, human intelligence has no match due to its versatility. E.g. the abilities to:

- Reason
- Achieve goals
- Understand and generate languages
- Perceive and respond to sensory inputs
- Prove mathematical theorems
- Play challenging games
- Synthesize and summarize information
- Create art and music
- Write histories

This makes human intelligence a natural choice for benchmarking the progress of AI.
You could even say that any activity computers are able to perform and people once performed, should be counted as an instance of intelligence. But matching any human ability is only a sufficient condition, not a necessary one as there are many systems already that exceed human intelligence. At least in speed at doing things!

The long and successful quest of AI to beat human players in chess, offered a high-profile instance for comparing human- to machine intelligence. Alan Turing mentioned the idea of computers showing intelligence with chess as a paradigm.

The final push was when IBM’s Deep Blue program beat Kasparov, the world chess champion. The publication itself never mentioned the word ‘intelligent’, but the frontier sure had moved.


## An operational definition

AI can also be defined by what AI researchers do. 
Firstly, it’s seen as a branch of computer science that studies the properties of intelligence by synthesizing intelligence. AI came from a dependency on hardware progress, but now the focus lies on software. 


This report views AI primarily as a branch of computer science that studies the properties of intelligence by synthesizing intelligence.10 Though the advent of AI has depended on the rapid progress of hardware computing resources, the focus here on software reflects a trend in the AI community. More recently, though, progress in building hardware tailored for neural-network-based computing has created a tighter coupling between hardware and software in advancing AI.

 “Intelligence” remains a complex phenomenon whose varied aspects have attracted the attention of several different fields of study, including psychology, economics, neuroscience, biology, engineering, statistics, and linguistics. Naturally, the field of AI has benefited from the progress made by all of these allied fields. For example, the artificial neural network, which has been at the heart of several AI-based solutions was originally inspired by thoughts about the flow of information in biological neurons.

