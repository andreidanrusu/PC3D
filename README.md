# NeRF-like reconstruction Prototype of 2D images (Work in progress)


A prototype I made to learn Instant-NGP pipelines.
This consists of:

 - Simple hash grid implementation with adjustable parameters (hash size, cell size, dimensions) and hashing
 - Image pre processing that essentially flattens images into a vector so they can be used by the MLP for backpropagation and splits them in batches
 - Very basic 3 layer MLP 
 - A multi res hash grid that combines multiple hash grids of various configurations based on the passed layout
 - A trainer that combines the implementations from above, compares the predicted feature vectors with the passed image, trains for a given number of iterations and reconstructs the image
   
The learning processes and some code segments were facilitated by ChatGPT.
