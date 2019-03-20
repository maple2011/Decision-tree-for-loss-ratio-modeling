# Decision-tree-for-loss-ratio-modeling

When target is loss ratio (i.e. loss$/premium), tree based model needs to apply premium as weight or frequency. Loss ratio concept is widely 
used in insurance and underwriting. Loss ratio can be calculated at group level (i.e. a group of customers) or at each customer level(i.e. each 
policy or customer). As a result, when rolling up loss ratio from customer level to group level, the weight/frequency are required. For example, 
in regression tree when the target variable is loss ratio, the loss ratio at root (of tree) is the total loss$/total premium. As the tree split, 
the loss ratio are calculated at each tree note and leaf. If the tree split until to individual level, then loss ratio becomes loss/premium of each 
customer. Therefore, a correct way to apply decisio tree is to apply weight/frequency.
