On a small test corpus, consisting of the letters
'b', 'a', 'i', 'd', 'k', and 'e', the HMM easily distinguishes the 
vowels from the consonents. However, on the larger Brown corpus, the
pattern is more unclear. This may have to do with the randomization of the 
initial parameters, as the Baum-Welch algorithm highly depends on these because
it is only suitable for local maxima, not global maxima. 
As of now, the code runs for 100 iterations on the first
1000 words of the Brown Corpus. If time allows, I will tinker with the 
initial, randomized parameter values to see if the HMM can distinguish between
vowels and consonents.

My code allows for arbitrary states and arbitrary alphabets to be run through the HMM,
as the HiddenMarkov class is defined for arbitrary lists. 
