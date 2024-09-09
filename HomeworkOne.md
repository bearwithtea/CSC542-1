## Question
> <img width="902" alt="Screenshot 2024-09-09 at 10 05 44 AM" src="https://github.com/user-attachments/assets/671e86c2-42f4-4a51-bde6-de8f3c38075e">
>
> a. Find the ID and name of each instructor in the Physics department.
>
> b. Find the ID and name of each instructor in a department located in the building “Watson”.
>
> c. Find the ID and name of each student who has taken at least one course in the “Comp. Sci.” department.
> 
> d. Find the ID and name of each student who has taken at least one course section in the year 2018.
> 
> e. Find the ID and name of each student who has not taken any course section in the year 2018.
## Answer
>
>a. $\pi_{\text{ID, name}}\left( \sigma_{\text{dept name = 'Physics'}}(\text{INSTRUCTOR}) \right)$
>
>b. $\pi_{\text{ID, name}}\left(\text{INSTRUCTOR} \bowtie_{\text{ instructor.deptname } = \text{ department.deptname}} \sigma_{\text{ building } = \text{ ``Watson''}}(\text{DEPARTMENT})\right)$
>
>c.  $\pi_{\text{ID, name}} \left( \text{COURSE} \bowtie_{\text{ student.id } = \text{ course.deptname } = \text{ ``Comp. Sci.''}} \left( \text{STUDENT} \right) \right)$
>
>d. $\pi_{\text{ID, name}} \left( \text{STUDENT} \bowtie_{\text{ student.id } = \text{ takes.id }} \sigma_{\text{ year } = 2018 } (\text{TAKES}) \right)$
>
>e. $\pi_{\text{ID, name}} \left( \text{STUDENT} \bowtie_{\text{ student.id } = \text{ takes.id }} \sigma_{\text{ year } ≠ 2018 } (\text{TAKES}) \right)$
