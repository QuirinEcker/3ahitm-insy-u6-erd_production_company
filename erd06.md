# ERD06 - Production Company


## Martin Notation
![](/Users/quirin/Documents/3AHITM/Informationssysteme/Uebungen/ERD06/erd06.png)

## Relations
Foreign-Key = *_id_*
Primary-Key = **_id_**

Employee=(**_employeeID_**, name, salary, _*machineID*_)
Machine=(**_machineID_**, name, _*employeeID*_, _*departmentID*_)
Department=(**_departmentID_**, name, *_HeadOfDepartment(employeeID)_*)
Part=(**_partNumber_**, description, _*parentPart(productionID)*_, _*neededInProduction*_);
Production=(**_productionID_**, speed, _*employeeID*_, _*machineID*_)
