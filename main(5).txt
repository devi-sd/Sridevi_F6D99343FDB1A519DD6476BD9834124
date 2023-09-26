class students:
  def __init__(self,name,roll_number,cgpa):
   self.name = name
   self.roll_number = roll_number
   self.cgpa = cgpa
def sort_students(student_list):
 sorted_students = sorted(student_list,key=lambda student:student.cgpa,reverse=True)
 return sorted_students
students =[students("Hari","3456",7.8),students("Srikanth","3457",8.9),students("Saumya","3458",8.9),students("Mahindhar","3459",9.9)]
sorted_students = sort_students(students)
for student in sorted_students:
 print("Name:{},Roll Number:{},CGPA:{}".format(student.name,student.roll_number,student.cgpa))
