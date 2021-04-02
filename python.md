- Python Trim String – rstrip(), lstrip(), strip()

- np.random.seed(0) and random.seed(0) only work for their own rng

- np.testing.assert_equal() can compare two objects that can contains arrays and return None if they are equal. Be aware 'assert' statment in testing require True/False return value. Thus, in testing, write "np.testing.assert_equal() is None"

- even when you are importing just one function from a file, it will run the entire file. So make sure all operations are under if __name__ == '__main__':

- working directory of unit test file is default to its location.  Use os.chdir(path)  to change it

- name of folder don't start with number, e.g use "a1" instead of "1"

if use "1", importing will not work


- cannot save csv file as csv-utf8

have to save it as just plain csv