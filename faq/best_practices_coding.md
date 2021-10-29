
# FAQ 

## What is the problem with the following code and what is the correct way ? 

````
    if @contract.save!
      redirect_to some_path, notice: t(".success")
    else
      render :new
    end
````

### Answer 
