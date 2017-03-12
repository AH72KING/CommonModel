# Common Model
All Credit goes to <a href="https://github.com/pakistanihaider"> Syed Haider Hassan #pakistanihaider @pakistanihaider </a>

PHP Framework Codeigniter Common Model
This Model is developed to use CodeIgniter CRUD functions to remove repetition and increase productivity as well as DRY ( Don't Repeat YourSelf ) Approach .

If you are fade up with use of this DB

<code> $this->DB... </code>

Use Common Model once  . you will never do this->db again. 
Common Model is easy to use and can be extended.


## How To Use 
Add the Common_model.php in model folder 
and add this line in your base controller or where you like to access DB best option is to add it into auto load.

<code> $this->load->model("Common_model"); </code>


## Select

<code> $this->Common_model->select('Table_Name_Here'); </code> 

this will give you object array of all fields of that table

### Select Fields
<code> $this->Common_model->select_fields('Table_Name_Here', 'Name, Age'); </code> 

for full parameters of select_fields function see common model file
select_fields($tbl = '', $data, $single = FALSE,$group_by = '',$order_by = '',$resultArray = false)

### Select Fields Where

<code> $this->Common_model->select_fields_where('Table_Name_Here' ,'Name, Age' ,'Age > 24'); </code> 

for full parameters of select_fields_where function see common model file
select_fields_where($tbl = '', $data, $where, $single = FALSE, $like = '', $field = '', $value = '',$group_by = '',$order_by = '',$array = false)


## Insert Record
<code> $this->Common_model->insert_record($tbl, $data); </code> 


## Update
<code> $this->Common_model->update($tbl, $where, $data) </code> 


## Delete
<code> $this->Common_model->delete($table , $where=NULL) </code> 


There is alot more in file Explore it you will love it 

