Feature B
=========

Level 2
-------

Level 3
^^^^^^^

Level 4
"""""""

1. item 1
2. item 2
#. item 3
#. item 4

====== ====== 
No.    Prime
====== ====== 
1      No
2      Yes
3      Yes
4      No
====== ====== 

The following is a code block::
  
  def hello():
      print("Hello world")


.. code-block:: c

   #include <stdio.h>
   int main()
   {
      printf("Hello, World!");
      return 0;
    }

.. code-block:: fortran

    subroutine Multiply(B,DI,Dix)
      type(sparse_matrix_diag),intent(in)::B
      type(diff_op),intent(in)           :: DI
      type(diff_op),intent(inout)           :: DIx
      integer::i,j,N
      real(kind=dp)::EPS
      real(kind=ddp),allocatable,dimension(:,:)::DIM

       N = DI%size
       EPS = epsilon(1.0_dp)
       allocate(DIM(N,N))

       DIM = 0.0_ddp
       call full(DI,DIM)
    end subroutine Multiply


.. #literalinclude
