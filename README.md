# CSARCH2 S01 -- Group 4

## The Password Life Cycle - Behind the Scenes of Encryption, Hashing and Secure Storage

HIZON, Allen Conner C.

INFANTE, Charles Sebastian V.

MARQUEZ, Jose Miguel S.

SY, Justin John Abraham F.

TENORIO, Jeroen Ralph I.

## 1.  Topic Theme

**An in-depth dive into the "password life cycle" - what actually
happens inside a computer system when handling passwords?**

The topic deals with the underlying computer architecture principles related to passwords’ handling, security, and compromising, Specifically, this deep dive starts with exploring client-side operations when allocating plaintext in volatile memory (RAM) and its encryption by the CPU to perform a safe TLS handshake and encrypt information prior to its further network transmission. At the backend, the topic is dedicated to server-side resource management when salt and hashes are being computed. This analysis would include comparison between architectural peculiarities of different hashing algorithms including the memory hardness of Argon2 as compared to SHA-1. It will include a comparison of the strengths and weaknesses of these algorithms as well as the specific characteristics that make an algorithm outshine the rest for handling passwords.

Apart from that, the topic will also explain the hardware aspects of storing encrypted hashes in non-volatile memory. Furthermore, the topic will break down the real-time computational flow during login verification. This includes the process of retrieving the stored salt and using the CPU for carrying out the comparison process to avoid side-channel attack through the use of the computer’s hardware component. Finally, the topic will include what happens to a password after it is stored in the database - how login attempts are verified, how a password gets reset, and even what happens if the database is compromised.

## 2.  Tech Stack Plan

### A.  Tech Stack

- Node.js 26

- Astro 6

- React

- TypeScript

- MDX

- Tailwind CSS

- Framer Motion

- HTML5

- CSS3

### B.  Interactive Element

The primary interactive element is a detailed simulation of the “life cycle” of a password. With animations and transitions between notable stages, the simulation will illustrate exactly what happens behind the scenes when a user creates a new account and password on a website.

Starting with a password inputted by the user accessing the exhibit, the simulation will display how the password is sent to the website over encrypted HTTPS, additionally explaining the potential security risks of not using encrypted communication when sending your password to the website.

After the website receives the password, the simulation will shift focus to what exactly the website does with your password behind the scenes. It will display an in-depth breakdown of the password hashing and salting process and explain why it’s necessary.

Additional interactive elements here would be used to help visualize different elements of the process. For example, an interactive preview of the security of different hashing algorithms or levels of compute. The user chooses between hash algorithms and how much RAM they want to allocate, and sees the corresponding time it would take to brute-force a hashed password update according to their choices.

After securely hashing and storing the password, the final stages of the simulation would focus on what happens next and the potential endings of a password’s life. It will show how the stored password hash is used to verify future login attempts, and what ultimately happens to a password in the event it is reset or the database is compromised by an external party.

### C. Mobile-responsive layout

The website will be usable and responsive on mobile devices due to the lack of advanced features that would necessitate a desktop device. There will be no intensive calculations on the client side, and the layout of the simulation and controls can easily be adjusted to accommodate for mobile devices given the chosen technologies like Tailwind CSS and React. 

## 3.  Tentative Style

The following is a series of mockup illustrations aiming to conceptualize the look and feel of the interactive exhibit. The final exhibit will have both media elements involving motion such as animations along with the potential for user interaction through forms accepting user input.

![](./images/media/image6.jpg)

![](./images/media/image5.jpg)

![](./images/media/image19.jpg)

![](./images/media/image24.jpg)

![](./images/media/image7.jpg)

![](./images/media/image15.jpg)

![](./images/media/image2.jpg)

![](./images/media/image17.jpg)

![](./images/media/image22.jpg)

![](./images/media/image11.jpg)

![](./images/media/image13.jpg)

![](./images/media/image4.jpg)

![](./images/media/image18.jpg)

![](./images/media/image26.jpg)

![](./images/media/image3.jpg)

![](./images/media/image8.jpg)

![](./images/media/image10.jpg)

![](./images/media/image21.jpg)

![](./images/media/image20.jpg)

![](./images/media/image9.jpg)

![](./images/media/image12.jpg)

![](./images/media/image14.jpg)

![](./images/media/image25.jpg)

![](./images/media/image23.jpg)

![](./images/media/image1.jpg)

![](./images/media/image16.jpg)
