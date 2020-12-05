# Polynomial-addition-using-Singly-Linked-List
Implementation of polynomial addition using Singly Linked List

Algorithm: 

1: start 

2: structure node created

3: struct Node *start=NULL; 

4: read both polynomials 

    4.1: add node tmp 

    4.1: tmp->next=NULL; 

    4.3: start=tmp; 

    4.4: tmp->coeff = coeff;

    4.5: tmp->pow = exp; 

    4.6: tmp-> next = NULL; 

5: print polynomials 

	    5.1: while(tmp != NULL)    
        printf("%dX^%d", tmp->coeff, tmp->pow);
                        tmp = tmp->next;
                        if(tmp != NULL)
                        printf("+");
          
6: struct Node* p_start,*start,*q_start,*start,*r_start,*start
	
7: p_start=start,  q_start=start; 

8: while(p_start!=NULL && q_start!=NULL) 

	   8.1: tmp=new node 

	   8.2: tmp->next = NULL 

	   8.3: if(p_start->pow == q_start->pow)
       
              tmp->coeff = p_start->coeff+q_start->coeff;
                       tmp->pow = p_start->pow;
                       p_start = p_start->next;
                       q_start = q_start->next; 

           8.4: else if(p_start->pow > q_start->pow)                          
 	          tmp->coeff = p_start->coeff;     
                       tmp->pow = p_start->pow;
                       p_start = p_start->next;
	 
          8.5:else if(p_start->pow < q_start->pow)
         
                       tmp->coeff = q_start->coeff;
            	          tmp->pow = q_start->pow;
            	          q_start= q_start->next;

	  8.6: if(start=NULL)
                      start=tmp
                      r_start=tmp
                   else
                      r_start->next=tmp;
                      r_start=tmp; 

9: if(p_start!=NULL)
	    tmp=new node
	    tmp->next = NULL;
                 tmp->pow=p_start->pow;
                 tmp->coeff=p_start->coeff;
                 p_start=p_start->next;
                 r_start->next=tmp;
                 r_start=tmp;
	
10:if(q_start=NULL)
                10.1:  while(q_start!=NULL)
	      tmp->coeff = q_start->coeff;
                   tmp->pow = q_start->pow;
                   q_start = q_start->next;
                   r_start->next=tmp;
                   r_start=tmp;

11: print sum 

12: stop
	
