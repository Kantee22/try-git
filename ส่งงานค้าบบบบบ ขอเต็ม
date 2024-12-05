class ClassRoom:
    def __init__(self, grade=0, homeRoomTeacher="", numStudents=0):
        self.grade = grade
        self.homeRoomTeacher = homeRoomTeacher
        self.studentList = []
        self.numStudents = numStudents

    def get_student_no(self, n):
        return self.studentList[n-1]

    def add_student(self, student_name):
        if self.numStudents < 10:
            self.studentList.append(student_name)
            self.numStudents += 1
            return True
        else:
            return False

    def set_grade(self, grade):
        self.grade = grade

    def set_homeroom_teacher(self, homeRoomTeacher):
        self.homeRoomTeacher = homeRoomTeacher

    def set_student_list(self, studentList):
        if len(studentList) <= 10:
            self.studentList = studentList

    def set_num_student(self, numStudents):
        if numStudents <= 10:
            self.numStudents = numStudents

    def get_grade(self):
        return self.grade

    def get_homeroom_teacher(self):
        return self.homeRoomTeacher

    def get_student_list(self):
        return self.studentList

    def get_num_student(self):
        return self.numStudents

    def change_student(self, n, new_name):
        if self.numStudents >= n > 0:
            self.studentList[n-1] = new_name
            return True
        else:
            return False

    def remove_student(self, student_name):
        if student_name in self.studentList:
            self.studentList.remove(student_name)
            self.numStudents -= 1
            return True
        return False

    def remove_student_no(self, n):
        if self.numStudents >= n > 0:
            del self.studentList[n - 1]
            self.numStudents -= 1
            return True
        else:
            return False

    def __str__(self):
        return f"""Grade: {self.grade}
Homeroom Teacher: {self.homeRoomTeacher}
Students: {', '.join(self.studentList)}"""

