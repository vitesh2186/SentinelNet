The **NSL-KDD dataset** was loaded from Kaggle into the notebook for analysis. Since the dataset did not originally contain column names, appropriate attribute names were added. The dataset consists of **43** attributes/dimensions, including features such as duration, protocol_type, service, flag, src_bytes, dst_bytes, and the target variables outcome and level.

The dimension/shape of the the dataset is (125972, 43)

From the exploration of data, got to know that there are **43** attributes/dimensions, namely,
duration  
protocol_type                 
service                       
flag                         
src_bytes                      
dst_bytes           
land                     
wrong_fragment  
urgent                       
hot                          
num_failed_logins            
logged_in                    
num_compromised              
root_shell                   
su_attempted                 
num_root              
num_file_creations 
count                 
srv_count             
serror_rate               
srv_serror_rate           
rerror_rate               
srv_rerror_rate           
same_srv_rate            
diff_srv_rate            
srv_diff_host_rate       
dst_host_count           
dst_host_srv_count       
dst_host_same_srv_rate     
dst_host_diff_srv_rate     
dst_host_same_src_port_rate
dst_host_srv_diff_host_rate
dst_host_serror_rate       
dst_host_srv_serror_rate   
dst_host_rerror_rate   
dst_host_srv_rerror_rate
outcome
level   

To understand the dataset better, basic exploratory methods were applied:
•	head(), tail() → Previewed initial and final rows of the dataset.
•	describe() → Obtained statistical summaries of numerical features.
•	info() → Checked data types and memory usage.
•	isnull() → Verified presence of missing values (none detected).

****Class Distribution****
The binary attack label (binary_attack) was analyzed to study the distribution of normal vs. attack traffic.
•	A count plot was generated, showing the proportion of Normal (0) and Attack (1) traffic.
•	Normalized value counts highlighted class imbalance, indicating a higher representation of attack traffic compared to normal traffic.
