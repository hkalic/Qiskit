# Coding with Qiskit
Following along YT playlist "Coding with Qiskit"

https://www.youtube.com/playlist?list=PLOFEBzvs-VvrgHZt3exM_NNiNKtZlHvZi

- - -

[My comments on Episode 4](/comments.episode4.md)
Why is this so different from YT output?

---------------------------------------------------------------------------
Episode 5 error. Don't know why.
... and it took 5 min on real HW
---------------------------------------------------------------------------
KeyError                                  Traceback (most recent call last)
Cell In[13], line 17
     14 counts = data.cr3.get_counts()
     15 total_counts = data.cr3.num_shots
---> 17 prob_Bell = (counts['00'] + counts['11']) / total_counts
     19 list_Bell.append(prob_Bell)
     20 list_other.append(1-prob_Bell)

KeyError: '11'
- - -
Finally, I found the error.
I forgot to measure at the end of circuit. LoL

That's why my results are all the same. I think '11'.

The other thing, 
when I run the job for the 1st time, I got the same result as in the YT e5.
However, 2nd run i got totaly different results (check the plots).
The same backend with the same code with time difference of one hour.

:confused:
