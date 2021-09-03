# assignment2-naini

# Santhosh Naini

###### Inida

**India** might just be the most colorful country in the world. It's a land of otherworldly landscapes for travel -- from **stunning lakes** and endless rolling plains to the snow-capped **Himalayas** in the north. It's also home to wild **festivals**, **romantic mausoleums** and some of the most hectic cities in the world.

---

# Travelling Directions
1. Maryville to Nizamabad (India)
    1. Maryville to Kansas City (MCI)
    2. Kansas City to Chicago (ORD)
    3. Chicago to New Delhi (IGI)
    4. New Delhi to Hyderabad (RGI)
    5. Hyderabad to Nizamabad (Domestic)

- Peace
- Clothes
- Electronic Items
- Food Items
- Money

![Santhosh Naini](https://github.com/NWMSU-SN/assignment2-naini/blob/main/naini.jpg)

---

# Food/Drink that I would recommend to my friend
| Food/Drink | Location | Price |
| :---: | :---: | :---: |
| Grill Chicken | Hyderabad | $12 |
| Parota | Pista house | $15 |
| Maggie | DLF | $3 |
| shawarma | Hitechcity | $1 |
| Icecream | Creamstone | $2 |

---
# Pithy Quotes
>*"And the trush shall make you free"*<br/>
>*"With the past, I have nothing to do; nor with the future. I live now."* -*Ralph Waldo Emerson*<br/>


---
# Code Fencing 
>Geometry (from the Ancient Greek: γεωμετρία; geo- "earth", -metron "measurement") is, with arithmetic, one of the oldest branches of mathematics. It is concerned with properties of space that are related with distance, shape, size, and relative position of figures.[1] A mathematician who works in the field of geometry is called a geometer.

[Source Link for Description](https://en.wikipedia.org/wiki/Geometry)

```
struct point2d {
    ftype x, y;
    point2d() {}
    point2d(ftype x, ftype y): x(x), y(y) {}
    point2d& operator+=(const point2d &t) {
        x += t.x;
        y += t.y;
        return *this;
    }
    point2d& operator-=(const point2d &t) {
        x -= t.x;
        y -= t.y;
        return *this;
    }
    point2d& operator*=(ftype t) {
        x *= t;
        y *= t;
        return *this;
    }
    point2d& operator/=(ftype t) {
        x /= t;
        y /= t;
        return *this;
    }
    point2d operator+(const point2d &t) const {
        return point2d(*this) += t;
    }
    point2d operator-(const point2d &t) const {
        return point2d(*this) -= t;
    }
    point2d operator*(ftype t) const {
        return point2d(*this) *= t;
    }
    point2d operator/(ftype t) const {
        return point2d(*this) /= t;
    }
};
point2d operator*(ftype a, point2d b) {
    return b * a;
}

```