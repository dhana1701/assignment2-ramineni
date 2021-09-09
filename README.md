# assignment2-ramineni

# Dhanalakshmi Ramineni

###### Niagara Falls 

Niagara Falls so **impressive** is the amount of water flowing over. Most of the tallest falls in the world have very little water flowing over them. It's the combination of height and volume that makes Niagara Falls so **breathtaking**. 

---

### Route Map

1. Drive from Maryville to Kansas City Aiport
2. Board a flight to Buffalo
   1. Kansas City to Chicago
   2. Chicago to New York   
   3. New York to Buffalo
3. Take a ride from buffalo to Niagara Falls

* Cave of the Winds 
* Adventure Theater
* Maid of the Mist (boat ride to Horseshoe Falls)
  * Grace
  * Freedom
  * Seas the Day
  * Therapy
* Trolley
* Aquarium
  * Fishes
  * California sea-lions
  * sea-horses
  * harbor seals
  * freshwater turtles
* Discovery Center & Hiking Trails

 [AboutMe](https://github.com/dhana1701/assignment2-ramineni/blob/main/AboutMe.md)

---

| Food/Drinks | Location | Price (Inr) |
| ---| ---| ---: |
| Chicken Biryani | Hyderabad | 300 |
| Sandwitch | Subway | 250 |
| Chai | Tea Time | 150 |
| Chicken Burger | KFC | 450 |

---
### Quotes about Life

>“You only live once, but if you do it right, once is enough.” - *Mae West*
>
> “Many of life’s failures are people who did not realize how close they were to success when they gave up.” - *Thomas A. Edison*

---

> String hashing is the way to convert a string into an integer known as a hash of that string.
An ideal hashing is the one in which there are minimum chances of collision (i.e 2 different strings having the same hash).
> Next Steps... <https://www.geeksforgeeks.org/string-hashing-using-polynomial-rolling-hash-function/>

---

```
long long compute_hash(string const& s) {
    const int p = 31;
    const int m = 1e9 + 9;
    long long hash_value = 0;
    long long p_pow = 1;
    for (char c : s) {
        hash_value = (hash_value + (c - 'a' + 1) * p_pow) % m;
        p_pow = (p_pow * p) % m;
    }
    return hash_value;
}

```
link below <https://cp-algorithms.com/string/string-hashing.html>

