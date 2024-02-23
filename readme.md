
In this notebook I have seen how to grab some raw data and create some interesting charts using Pandas and Matplotlib. I have:

* used .groupby() to explore the number of posts and entries per programming language
* converted strings to Datetime objects with to_datetime() for easier plotting
* reshaped the DataFrame by converting categories to columns using .pivot()
* used .count() and isna().values.any() to look for NaN values in the DataFrame, which I then replaced using .fillna()
* created (multiple) line charts using .plot() with a for-loop
* styled the charts by changing the size, the labels, and the upper and lower bounds of the axis.
* added a legend to tell apart which line is which by colour
* smoothed out the time-series observations with .rolling().mean() and plotted them to better identify trends over time.


#################

My comment is limited to what I could see based on this data, based on the number of posts published on StackOverflow and grouped according to their respective tags (referring to programming languages) from 2008 to February 2024...

Once I cleaned the data and a projection of the post numbers per month for all languages was created on a timeline, I could clearly see the trend of various languages. For example, which language was the most popular during the x/y timeframe, which one had the fewest posts in a particular timeframe, which languages are the oldest, most recent, etc

What particularly interested me was observing the growth of Python and its staggering rise in popularity, especially since 2019, riding the AI narrative, reaching a figure of 29,378 posts in just the month of May 2020 (during the full period of government closures due to Covid).

Another phenomenon that I found interesting and peculiar was the downtrend starting from the second half of 2021 and adopting a steep decline from 2023. Certainly, to define the causes of such a phenomenon, cross-sectional studies would be needed, but I have to reasoning based on my personal experience.

At the beginning of my Python journey, in early 2023, my reference point was StackOverflow, W3schools, YouTube, etc... Over time (although I resisted this change somewhat, as I wanted to learn as others had learned before me, by banging my head against the problems and cases of other people on sites, blogs, and platforms like Discord, etc.), I ended up making a slow and then accelerated transition to ChatGPT, not just to copy and paste, but rather to have things explained to me and to reason about the things I didn't understand... And I noticed that indeed it was much more practical than the classic googling and trying to end up on StackOverflow... Of course, it still happens that I have to resort to StackOverflow, but much less... So, in summary (subjectively speaking), I think that the downtrend in the number of posts on StackOverflow is due to the mass arrival of technologies like ChatGPT, the arrival of new competitors to StackOverflow, as for the loss of peak numbers, I think this is due to the recapture of people's freedom after the pandemic, so they are not forced to spend hours in front of the PC looking for something to do, learn, or improve...


################## ITA ################

Il mio commento si limita solo a ciò che ho potuto vedere in base a questi dati, basati sul numero di post pubblicati su StackOverflow e raggruppati in base ai rispettivi tag (che si riferiscono ai linguaggi di programmazione) a partire dal 2008 fino a febbraio 2024...

Una volta puliti i dati e creato una proiezione dei numeri di post al mese di tutti i linguaggi su una linea temporale, ho potuto vedere chiaramente il trend dei vari linguaggi, ad esempio qual è il linguaggio che è stato il più popolare nell'arco temporale x/y, qual è quello che ha avuto meno post in un determinato lasso temporale, quali sono i linguaggi più vecchi, più recenti, ecc.

Ciò che mi ha interessato in particolare è stato osservare la crescita di Python e la vertiginosa crescita di popolarità in particolare dal 2019, cavalcando la narrativa dell'IA, raggiungendo la cifra di 29378 posts nel solo mese di maggio 2020 (pieno periodo chiusure governative motivante covid)

Un altro fenomeno che ho trovato interessante e particolare è stato il downtrend partito dalla seconda metà del 2021 e che ha adottato una caduta vertiginosa dal 2023. Certamente, per poter definire le cause di tale fenomeno servirebbe fare degli studi incrociati, ma devo ragionare sulla mia esperienza personale.

All'inizio del mio percorso, a inizio del 2023, il mio punto di riferimento era StackOverflow,  W3schools, YouTube, ecc... Con il tempo (anche se ho fatto non poca resistenza alla cosa, in quanto volevo imparare come avevano imparato gli altri prima di me, dunque sbattendo la testa su casi e problemi di altre persone sui siti, blog e piattaforme come Discord, ecc.), ho finito per fare una lenta e infine accelerata transizione su ChatGPT, non per fare ctrl+C e ctrl+V, ma bensì per farmi spiegare e ragionare sulle cose non capite... E ho notato che in effetti era molto più pratico rispetto al classico googlare e cercare di finire su StackOverflow... Certo, capita comunque di dover ricorrere a StackOverflow, ma molto meno... Dunque, in sintesi (soggettivamente parlando), penso che il downtrend dei numeri di post su StackOverflow sia dovuto all'arrivo in massa di tecnologie come ChatGPT, l'arrivo di nuovi competitor di StackOverflow, in quanto alla perdita del picci massimi, penso questo sia dovuto alla riconquista della liberta delle persone dopo la pandemia, dunque non mi costretti a passare ore davanti al pc in cerca di qualcosa da fare, imparare o migliorare.





