RESET & RENUMBER PRIMARY KEY
-------------------------------
SET @var_name = 0;
UPDATE client SET id = (@var_name := @var_name +1);
ALTER TABLE client AUTO_INCREMENT = 1