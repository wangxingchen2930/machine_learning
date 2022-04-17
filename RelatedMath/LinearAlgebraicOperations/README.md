# Geometry and Linear Algebraic Operations

## Vectors

- Commonly, the column will be used as default.

## dot product

To get angle using dot product:
```
def angle(v, w):
    return torch.acos(v.dot(w) / (torch.norm(v) * torch.norm(w)))
```

## Hyperplanes

In an d-dimensional vector space, a hyperplane has d-1 dimensions and divides the space into two half-spaces. 

- Hyperplanes are often referred to as decision planes that separate the different target classes.

## Matrix

- @ was used in python for matrix multiplication

## Linear Dependence

If there is no linear dependence we say the vectors are linearly independent.

- we can solve for one of the vectors in terms of some combination of the others, and effectively render it redundant. 
- Thus, a linear dependence in the columns of a matrix is a witness to the fact that our matrix is compressing the space down to some lower dimension. 

## Rank

The rank of a matrix A is the largest number of linearly independent columns amongst all subsets of columns

### Computationally efficient way to compute the rank of a matrix

(to be done)

## Invertibility

- Multiplication by a full-rank matrix (i.e., some A that is nxn matrix with rank n), we should always be able to undo it
- A quantity called the determinant, which has the property that as long as the determinant is not zero, we can find a solution.