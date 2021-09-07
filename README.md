# Assignment2-Venkatesh
# Venkatesh Guttikonda
###### Paris 
Paris was considered as a **city** of Love for the **world**


---

Directions From Maryville to Paris

1. Get a Flight ticket for flying 
    * Make it on time boarding  
2. Let's take a Goood Nap for Long Flight
    * Get a Nice and Peaceful sleep for 12hours
3. Get a taxi in Paris
     * 3.1 Start exploring the City Of Love
     * 3.2 Markdown the Places to Visit With Local Map

---

List of Items to get in Paris for getting Maximum enjoyment

* Make a Friends over there
* To Capture Every Moment as Memory then Get the Things like
   * Camera
   * Go Pro
   * Drones may be
* Get some real taste of French Dishes Like
   * Boeuf Bourguignon
   * Croque Monsieur
   * Pot au Feu       

   ---

  # You can Know me Here # 

   [Let's get to know Aboutme](Aboutme.md)

  ---

  ### Food I would recommend to try Once ###
  
  |   Food   |   Place   |   Price   |
  | -------- | --------- | --------- |
  | Sausage Mcmuffin | Mc Donalds | $1.19 |
  | Pepperoni Pizza | Hyvee | $5.19 |
  | 6 foot long Wrap | Subway | $6.99 |
  | Pizza Ranch Buffet | Pizza Ranch | $11.99 |

  ---
 
  ## Pithy Quotes ##

 **Happiness** is not something **ready** made. It comes from your **own actions**. - *Dalai Lama*

  Be *realistic*: **Plan** for a ***miracle***. - *Osho*

  ---

  *Combinatorics* is an area of **mathematics** primarily concerned with counting, both as a means and an end in obtaining results, and certain properties of **finite structures**. It is closely related to many other areas of mathematics and has many applications ranging from logic to **statistical physics**, from ***evolutionary biology***to *computer science*, etc.

  ### Link For the Description ###

  [Description of Combinatorics](https://en.wikipedia.org/wiki/Combinatorics)

  ```
  int solve (int n, int r) {
    vector<int> p;
    for (int i=2; i*i<=n; ++i)
        if (n % i == 0) {
            p.push_back (i);
            while (n % i == 0)
                n /= i;
        }
    if (n > 1)
        p.push_back (n);

    int sum = 0;
    for (int msk=1; msk<(1<<p.size()); ++msk) {
        int mult = 1,
            bits = 0;
        for (int i=0; i<(int)p.size(); ++i)
            if (msk & (1<<i)) {
                ++bits;
                mult *= p[i];
            }

        int cur = r / mult;
        if (bits % 2 == 1)
            sum += cur;
        else
            sum -= cur;
    }

    return r - sum;
}

```

### Link For Code Source ### 

[Link For Code Source](https://cp-algorithms.com/combinatorics/inclusion-exclusion.html)






