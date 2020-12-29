
### 連結的欄位
#### 1.同型別
#### 2.同長度

```
SELECT ksu_std_name, ksu_std_department, dept_name
FROM
ksu_std_table as a, dept_detail as b
WHERE
a.ksu_std_department = b.dept_id
```
#### 更改名稱dept_id 為ksu_std_department
```
ALTER TABLE dept_detail CHANGE
      dept_id
      ksu_std_department
      char(2);
```
