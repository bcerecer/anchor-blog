# Blog

This is a Blog program built with Anchor and the idea of this repo is to get practice on Solana's programs since this is not a feasible way to implement a blog as the space to store posts on chain can get expensive quick. 

## Design

- **Blog Account**

Each **Blog Account** is a PDA derived from the keyword "blog_v0" and the user's public key. 

- **Post Account**

Each **Post Account** is a PDA derived from the **Blog Account's** public key and the **Blog Account's** `post_count` value, which is the number of posts that such Blog Account has created. Also, each **Post Account** will be assigned 10kb of space.
