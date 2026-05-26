### House-Price-Prediction  
### ANALYSIS PHASE OF THE PROJECT  
  
**Systematically analysing the data structure and thourough accessing its inaccuracies**

#### Project Background and Overview
This readme shows the analytical stage of the real-estate predictive project which focus on understanding the data structure, features, economic and behaviorer factors influencing the prices and sales of the properties  

#### This phase was executed in order to:  
- inspect and validate data quality
- Detect and outliers 
- Understand relationship between variables  
- Understand what drive the business problem  
- Discover predictive patterns  
- Prepare the dataset for a predictive modelling  
  
**This phase was strictly executed to fit into into giving the dataset data quality that would prevent the models that would be built behind the data in the future to giving bias prediction**  

### Business Concern and Challenge  
**The real-estate pricing increasingly depend on:**   
- Automated Valuation Models
- Investment Intelligence
- Predictive Pricing Engine  
- Smart Property Recommendation System
  
**Nonetheless**  
In sccurate pricing model can result in:   
  
- Property Overvaluation  
- Investors' losses  
- Morgage risks exposure  
- Poor urban-planning decisions  
- Biased market prediction  
  
Therefore, the object of this project is to findout the features than drive residential housing pricing and determine how property features influence the final sale of the property  

The data contain structured residential housing record of 80 features explaining:  
- Property location
- Land characteristics
- Building structure
- Quality ratings
- Basement features
- Garage features
- Interior room composition
- Utilities
- Outdoor facilities
- Sales conditions.  
- And the target which is the `Salesprice`  
  
### Missing values and inconsistencies  
Missing values were analysed contexually rather than globally.

**Missing values in the categorical columns**
Several missing values in the categorical columns represent absence rather than missing information. Therefore, some missing values meant:   
`no pool`
`no alley`
`no garage`
`no basement`  
  
Therefore, instead of globally addressing or dealing with the null, they were rather filled with string called **`null`** and this preserved business meaning.  
  
**Missing values in the numerical columns were  handled through:**  
Inorder to assigned the data directly to the models to identify them as they are, the missing values in the numerical columns were filled with `int 0` indicating there were no quantity in that particular space and this method inproves confidence of the data integrity.  
  
Text values were standardized into lower case format to reduce:  
- duplicate labels
- inconsistencies representation  
- encoding instability  

Inorder for full understanding of the group to which each column belong to, some columns which have like-identity were grouped together into a general name.  
Example onclude:  
- Location and zoning.
The columns that were added are: Neighborhood, street, alley, mszoning, condition1, condition2  
  
Some other columns were also grouped to form one general representator of that group. Some are:    
`Lot Features`
`Lot Features`  
`Building Structure`  
`Quality/Condition`  
`Size and Space`  
`Basement Features`  
`Garage Features`  
`Rooms and Interior` 
`Extras and Outdoors`  
`Exterior`  
`Utilities`  
`Sales type and information` 
  
These give the full overview of the project features and understanding which group feature influence/drive the target which is saleprice. 

