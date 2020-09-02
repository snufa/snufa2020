The last years have seen many exciting new developments to train spiking neural networks to perform complex information processing. This online workshop brings together researchers in the field to present their work and discuss ways of translating these findings into a better understanding of neural circuits. Topics include artificial and biologically plausible learning algorithms and the dissection of trained spiking circuits toward understanding neural processing. We have a manageable number of talks with ample time for discussions.

The workshop is being organised by [Dan Goodman](https://neural-reckoning.org) and [Friedemann Zenke](https://fzenke.net/).

## Registration

Registration is required but free and open. [Register here](https://www.eventbrite.co.uk/e/spiking-neural-networks-as-universal-function-approximators-tickets-114419361390) and you will receive an email before the event with the Crowdcast/Zoom URL.

## Agenda

Talks will be 45m (30m + 15m questions/discussion). Hover over the talk titles to see abstracts (if one is available).

### August 31st

<script language="javascript">
	function LT(d, t) {
		var date = new Date(d+' 2020 '+t+' UTC+2');
		document.write(date.toString());
	}
</script>

Time (CET) | Session | Local date/time
-----------|---------|----------------
14:00 | Welcome by organizers | <script language="javascript">LT('31 Aug', '14:00')</script>
14:10 | **Sander Bohte** (CWI)<br/><span title="The emergence of brain-inspired neuromorphic computing as a paradigm for edge AI is motivating the search for high-performance and efficient spiking neural networks to run on this hardware. However, compared to classical neural networks in deep learning, current spiking neural networks lack competitive performance in compelling areas. Here, for sequential and streaming tasks, we demonstrate how spiking recurrent neural networks (SRNN) using adaptive spiking neurons are able to achieve state-of-the-art performance compared to other spiking neural networks and almost reach or exceed the performance of classical recurrent neural networks (RNNs) while exhibiting sparse activity. From this, we calculate a 100x energy improvement for our SRNNs over classical RNNs on the harder tasks. We find in particular that adapting the timescales of spiking neurons is crucial for achieving such performance, and we demonstrate the performance for SRNNs for different spiking neuron models.">Effective and Efficient Computation with Multiple-timescale Spiking Recurrent Neural Networks</span> | <script language="javascript">LT('31 Aug', '14:10')</script>
14:55 | **Iulia M. Comsa** (Google Research)<br/><span title="The timing of individual neuronal spikes is essential for biological brains to make fast responses to sensory stimuli. However, conventional artificial neural networks lack the intrinsic temporal coding ability present in biological networks. We propose a spiking neural network model that encodes information in the relative timing of individual neuron spikes. In classification tasks, the output of the network is indicated by the first neuron to spike in the output layer. This temporal coding scheme allows the supervised training of the network with backpropagation, using locally exact derivatives of the postsynaptic spike times with respect to presynaptic spike times. The network operates using a biologically-plausible alpha synaptic transfer function. Additionally, we use trainable synchronisation pulses that provide bias, add flexibility during training and exploit the decay part of the alpha function. We show that such networks can be trained successfully on noisy Boolean logic tasks and on the MNIST dataset encoded in time. The results show that the spiking neural network outperforms comparable spiking models on MNIST and achieves similar quality to fully connected conventional networks with the same architecture. We also find that the spiking network spontaneously discovers two operating regimes, mirroring the accuracy-speed trade-off observed in human decision-making: a slow regime, where a decision is taken after all hidden neurons have spiked and the accuracy is very high, and a fast regime, where a decision is taken very fast but the accuracy is lower. These results demonstrate the computational power of spiking networks with biological characteristics that encode information in the timing of individual neurons. By studying temporal coding in spiking networks, we aim to create building blocks towards energy-efficient and more complex biologically-inspired neural architectures.">On temporal coding in spiking neural networks with alpha synaptic function</span> | <script language="javascript">LT('31 Aug', '14:55')</script>
15:40 | Break (30mins) | <script language="javascript">LT('31 Aug', '15:40')</script>
16:10 | **Franz Scherr** (TUG)<br/><span title="Transformative advances in deep learning, such as deep reinforcement learning, usually rely on gradient-based learning methods such as backpropagation through time (BPTT) as a core learning algorithm. However, BPTT is not argued to be biologically plausible, since it requires to a propagate gradients backwards in time and across neurons. Here, we propose e-prop, a novel gradient-based learning method with local and online weight update rules for recurrent neural networks, and in particular recurrent spiking neural networks (RSNNs). As a result, e-prop has the potential to provide a substantial fraction of the power of deep learning to RSNNs. In this presentation, we will motivate e-prop from the perspective of recent insights in neuroscience and show how these have to be combined to form an algorithm for online gradient descent. The mathematical results will be supported by empirical evidence in supervised and reinforcement learning tasks. We will also discuss how limitations that are inherited from gradient-based learning methods, such as sample-efficiency, can be addressed by considering an evolution-like optimization that enhances learning on particular task families. The emerging learning architecture can be used to learn tasks by a single demonstration, hence enabling one-shot learning.">E-prop: A biologically inspired paradigm for learning in recurrent networks of spiking neurons</span> | <script language="javascript">LT('31 Aug', '16:10')</script>
16:55 | **Emre Neftci** (UC Irvine)<br/><span title="The potential of machine learning and deep learning to advance artificial intelligence is driving a quest to build dedicated computers, such as neuromorphic hardware that emulate the biological processes of the brain. While the hardware technologies already exist, their application to real-world tasks is hindered by the lack of suitable programming methods. Advances at the interface of neural computation and machine learning showed that key aspects of deep learning models and tools can be transferred to biologically plausible neural circuits. Building on these advances, I will show that differentiable programming can address many challenges of programming spiking neural networks for solving real-world tasks, and help devise novel continual and local learning algorithms. In turn, these new algorithms pave the road towards systematically synthesizing machine intelligence in neuromorphic hardware without detailed knowledge of the hardware circuits.">Synthesizing Machine Intelligence in Neuromorphic Computers with Differentiable Programming</span> | <script language="javascript">LT('31 Aug', '16:55')</script>
17:40 | Break (30mins) | <script language="javascript">LT('31 Aug', '17:40')</script>
18:10 | **Discussion (can continue as long as needed)**<br/><span title="How large do we need SNNs to be and how do we train them to do our research? What are the next steps the field should take to swiftly move forward?">Current technical constraints and bottlenecks.</span><br/><span title="How do we leverage this methodological advance to gain a better understanding of how the brain processes information? What constitutes a conceptual advance? And how do we compare trained spiking neural networks to biology?">We can train spiking neural networks. What now?</span> | <script language="javascript">LT('31 Aug', '18:10')</script>

### September 1st

Time (CET) | Session | Local date/time
-----------|---------|----------------
14:00 | Welcome by organizers | <script language="javascript">LT('1 Sep', '14:00')</script>
14:10 | **Timothee Masquelier** (CNRS Toulouse)<br/><span title="Back-propagation is a powerful supervised learning algorithm in artificial neural networks, because it solves the credit assignment problem (essentially: what should the hidden layers do?). This algorithm has led to the deep learning revolution. But unfortunately, back-propagation cannot be used directly in spiking neural networks (SNN). Indeed, it requires differentiable activation functions, whereas spikes are all-or-none events which cause discontinuities. Here we present two strategies to overcome this problem. The first one is to use a so-called 'surrogate gradient', that is to approximate the derivative of the threshold function with the derivative of a sigmoid. We will present some applications of this method for time series processing (audio, internet traffic, EEG). The second one concerns a specific class of SNNs, which process static inputs using latency coding with at most one spike per neuron. Using approximations, we derived a latency-based back-propagation rule for this sort of networks, called S4NN, and applied it to image classification.">Back-propagation in spiking neural networks</span> | <script language="javascript">LT('1 Sep', '14:10')</script>
14:55 | **Claudia Clopath** (Imperial College)<br/>Training spiking neurons with FORCE to uncover hippocampal function | <script language="javascript">LT('1 Sep', '14:55')</script>
15:40 | Break (30mins) | <script language="javascript">LT('1 Sep', '15:40')</script>
16:10 | **Richard Naud** (U Ottawa)<br/><span title="Synaptic plasticity is believed to be a key physiological mechanism for learning. It is well-established that it depends on pre and postsynaptic activity. However, models that rely solely on pre and postsynaptic activity for synaptic changes have, to date, not been able to account for learning complex tasks that demand hierarchical networks. Here, we show that if synaptic plasticity is regulated by high-frequency bursts of spikes, then neurons higher in the hierarchy can coordinate the plasticity of lower-level connections. Using simulations and mathematical analyses, we demonstrate that, when paired with short-term synaptic dynamics, regenerative activity in the apical dendrites, and synaptic plasticity in feedback pathways, a burst-dependent learning rule can solve challenging tasks that require deep network architectures. Our results demonstrate that well-known properties of dendrites, synapses, and synaptic plasticity are sufficient to enable sophisticated learning in hierarchical circuits.">Burst-dependent synaptic plasticity can coordinate learning in hierarchical circuits</span> | <script language="javascript">LT('1 Sep', '16:10')</script>
16:55 | **Julian Goeltz** (Uni Bern)<br/><span title="Engineered pattern-recognition systems strive for short time-to-solution and low energy-to-solution characteristics. This represents one of the main driving forces behind the development of neuromorphic devices. For both them and their biological archetypes, this corresponds to using as few spikes as early as possible. The concept of few and early spikes is used as the founding principle in the time-to-first-spike coding scheme. Within this framework, we have developed a spike-timing-based learning algorithm, which we used to train neuronal networks on the mixed-signal neuromorphic platform BrainScaleS-2. We derive, from first principles, error-backpropagation-based learning in networks of leaky integrate-and-fire (LIF) neurons relying only on spike times, for specific configurations of neuronal and synaptic time constants. We explicitly examine applicability to neuromorphic substrates by studying the effects of reduced weight precision and range, as well as of parameter noise. We demonstrate the feasibility of our approach on continuous and discrete data spaces, both in software simulations and on BrainScaleS-2. This narrows the gap between previous models of first-spike-time learning and biological neuronal dynamics and paves the way for fast and energy-efficient neuromorphic applications.">Fast and deep neuromorphic learning with time-to-first-spike coding</span> | <script language="javascript">LT('1 Sep', '16:55')</script>
17:40 | Break (30mins) | <script language="javascript">LT('1 Sep', '17:40')</script>
18:10 | **Discussion (can continue as long as needed)**<br/><span title="Neurons communicate via precisely timed, discrete pulses rather than by analogue signals. Why? Is there a computational advantage to this mode of communication, or is just to save energy? With the recent advances in our ability to train spiking neural networks discussed in this workshop, can we throw new light on this age old discussion, and outline a programme to resolve it?">Why spiking?</span> | <script language="javascript">LT('1 Sep', '18:10')</script>

## Discussion topics

### Monday, August 31

We will discuss two topics:

**Current technical constraints and bottlenecks.**

How large do we need SNNs to be and how do we train them to do our research? What are the next steps the field should take to swiftly move forward?

**We can train spiking neural networks. What now?**

How do we leverage this methodological advance to gain a better understanding of how the brain processes information? What constitutes a conceptual advance? And how do we compare trained spiking neural networks to biology?

### Tuesday, September 1

**Why spiking?**

Neurons communicate via precisely timed, discrete pulses rather than by analogue signals. Why? Is there a computational advantage to this mode of communication, or is just to save energy? With the recent advances in our ability to train spiking neural networks discussed in this workshop, can we throw new light on this age old discussion, and outline a programme to resolve it?
