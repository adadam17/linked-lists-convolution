# Linked lists convolution

Browser app that builds a linked list L3 from two linked lists L1 = a1..an and L2 = b1..bn, where

c_k = a1·b_k + a2·b_(k−1) + … + a_k·b1, for k = 1..n

Two versions, each with its running time in milliseconds:

- **Singly linked lists**: the lists are never reversed. The product a_i·b_j is added to c_(i+j−1), so every pointer only moves forward. Θ(n²).
- **Doubly linked lists**: c_k is computed directly, with one pointer moving forward on L1 and one moving backward (`prev`) on L2 from b_k. Θ(n²).

Single HTML file, no installation: open `index.html` in any browser.
