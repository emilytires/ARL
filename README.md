# ASSOCIATION RULE LEARNING

   Association Rule Learning is a rule based algorithm. It is discovering pattern of items, products or movies. The most commonly used association analysis algorithm is Apriori. Let's dive into Apriori metrics.

Antecedents and Consequent

   The IF component of an association rule is known as the antecedent. The THEN component is known as the consequent. The antecedent and the consequent are disjoint; they have no items in common. They can be single item or more items.

Antecedent Support

   Probability of antecedent observed alone in all market

Consequent Support

   Probability of consequent observed alone in all market

Support

   The support of a rule indicates how frequently the items in the rule occur together. For example, beer and milk might appear together in 40% of the transactions. If so, the following two rules would each have a support of 40%.
  
 Confidence
 
   The confidence of a rule indicates the probability of both the antecedent and the consequent appearing in the same transaction. Confidence is the conditional probability of the consequent given the antecedent. For example, beer appear in 50 transactions; 40 of the 50 might also include milk. The rule confidence would be:

beer implies milk with 80% confidence

Lift

   Both support and confidence must be used to determine if a rule is valid. However, there are times when both of these measures may be high, and yet still produce a rule that is not useful.
  
Our Script Steps:

  1- Data Preprocessing
  
  2- Segments customers into 3 groups to using Customer Lifetime Prediction method
  
  3- Create 3 data set according to the user ids of the 3 segments (for example for 3 segments: a_segment_df, b_segment_df, c_segment_df)
  
  4- Create invoice-product matrix association rules for each segment
  
  5- Rrecommendations for German Customers by their segment
  
 
 References:
 
 https://docs.oracle.com/cd/E18283_01/datamine.112/e16808/algo_apriori.htm
