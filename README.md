                                             (HOSPITAL MANAGAMENT)
create database shree_hospital;
use shree_hospital;

create table Patient(
patient_id int,
patient_first_name varchar(255) not null,
patient_last_name varchar(255) not null,
gender varchar(255)not null,
address varchar(255) not null,
room_no int not null,
date_of_admit int not null,
date_of_dicharge int not null,
doctor_id int not null,
disease varchar(255) not null,
primary key (patient_id));

insert into patient
value(1, 'rani', 'patil', 'f', 'kalyan', 1, 20-5-13, 23-5-13, 1, 'chest_pain'),
(2, 'sunita', 'jadhav', 'f', 'thane', 4,  22-5-13, 29-5-13, 2, 'chicken_pox'),
(3, 'anita', 'pawshe', 'f', 'kalwa', 3, 23-5-13, 25-5-13, 3,'skin_cancer'),
(4, 'manish', 'rane', 'm', 'thakurli', 5, 24-4-13, 31-5-13, 8, 'stomch_issuse'),
(5, 'vaibhav', 'rane', 'm', 'ulhasnager', 7, 24-5-13, 1-6-13, 15, 'food_poisoing'),
(6, 'hemant', 'durge', 'm', 'panvel', 6, 28-5-13, 3-6-13, 4, 'hay_fever'),
(7, 'abhinav', 'parte', 'm', 'badlapur', 5, 29-5-13, 4-6-13, 5, 'headaches'),
(8, 'sunil', 'thorve', 'm', 'karjat', 3, 31-5-13, 4-6-13, 7, 'hearing_loss'),
(9, 'ankita', 'vichare', 'f', 'badlapur', 7, 1-6-13, 9-6-13, 22, 'rentinal_detachment'),
(10, 'anshika', 'rane', 'f', 'karjat', 9, 2-6-13, 4-6-13, 21 ,'itching'), 
(11, 'ram', 'patil', 'm', 'neral', 3, 2-6-13, 7-6-13, 17, 'kidney_infection'),
(12, 'pooja', 'yadav', 'f', 'bhivpuri', 6, 5-6-13, 9-6-13, 31, 'kidney_stone'),
(13, 'seeta', 'mishra', 'f', 'kalwa', 3, 6-6-13, 7-8-13, 12, 'cough'),
(14, 'geeta', 'sharma', 'f', 'vangani', 4, 6-6-13, 10-6-13, 11, 'itching'),
(15, 'ram', 'chavan', 'm', 'kalyan', 10, 6-6-13, 13-6-13, 10, 'leg_cramps'),
(16, 'manisha', 'farnandez', 'f', 'kalwa', 11, 14-6-22, 14-6-13, 41, 'liver_dises'),
(17, 'ravikant','mishra', 'm', 'panvel', 14, 18-6-13, 28-6-13, 33, 'maleria'),
(18, 'ajnali', 'shelke', 'f','aroli',  15, 18-6-13, 19-6-13, 47, 'migrane'),
(19, 'narendra', 'gupta', 'm', 'uran', 12, 20-6-13, 28-6-13, 18, 'mouth_ulcer'),
(20, 'devenrda', 'pandit', 'm', 'nagpur', 17, 21-6-13, 30-6-13, 19, 'central_core_diesease'),
(21, 'jayendra', 'koli', 'm', 'bhandup', 19, 27-6-13, 30-6-13, 13, 'obesity'),
(22, 'vishwanath', 'ayer', 'm', 'vikroli',17, 27-6-13, 1-7-13, 50,  'osteoarthritis'),
(23, 'pranali', 'sonawane', 'f', 'pune', 2, 28-6-13, 8-7-13, 9, 'covid19'),
(24, 'dipak', 'pande',  'm', 'lonawala', 4, 9-6-13, 12-6-13, 10,'maleria'),
(25, 'sanjay', 'chandrashekhar', 'm', 'amrawati', 5, 10-6-13, 23-6-13, 44, 'middle_year_infection'),
(26, 'aman', 'sharma', 'm', 'karjat',6, 11-6-13, 15-6-13, 19, 'panic_disorder'),
(27, 'ruksana', 'shaikh', 'f', 'neral', 4, 11-6-13, 28-6-13, 13, 'back_and_neck_pain'),
(28, 'rudra', 'thakur', 'm', 'ulhasnagar', 2, 15-6-13, 26-6-13, 4, 'glaucma'),
(29, 'gautami', 'barve', 'f', 'dombivali', 3, 20-6-13, 27-6-13, 6, 'teeth_infection'),
(30, 'alka', 'jadhav', 'f', 'lonawala', 8, 23-6-13, 30-6-13, 10, 'dengu'),
(31, 'ranu','mandal', 'f', 'kalwa', 7,23-6-13, 29-6-13, 17, 'migrane'),
(32, 'sony', 'pawar', 't', 'kalyan', 6, 30-6-13, 1-7-13, 6, 'misaligned_teeth'),
(33, 'kamal', 'pawar', 'f', 'dombivali',9, 3-7-13, 7-7-13, 8, 'stomach_pain'),
(34, 'seeta', 'manrai', 'f', 'kalyan', 4, 4-7-13, 12-7-13, 45, 'emphysema'),
(35, 'hasina', 'parkar', 'f', 'nagpur', 7, 7-7-13, 12-7-13, 3, 'psoriasis'),
(36, 'rambhau', 'ovhal', 'm', 'kalyan', 3, 12-7-13, 17-7-13, 7, 'maleria'),
(37, 'geeta', 'shinde', 'f', 'kalyan', 3, 13-7-13, 18-7-13, 3, 'eczema'),
(38, 'ram', 'iyer', 'm', 'dombivali', 3, 21-7-13, 22-7-13, 5, 'back_and_neck_pain'),
(39, 'sharan', 'kumar', 'm', 'bandra', 3, 24-7-13, 27-7-13, 4, 'astigmatism'),
(40, 'siddharth', 'shah', 'm', 'kandivali', 6, 12-8-13, 16-8-13, 7, 'maleria'),
(41, 'komal', 'jadhav', 'f', 'parel', 2, 12-8-13, 17-8-13, 18, 'cholera'),
(42, 'shraddha', 'gurav', 'f', 'colaba', 5, 14-8-13, 18-8-13, 14, 'dengue'),
(43, 'tejal', 'padwale', 'f', 'ambernath', 7, 15-8-13, 20-8-13, 12, 'constipation'),
(44, 'prajakta', 'hande', 'f', 'bhiwandi', 8, 17-8-13, 121-8-13, 11, 'obesity'),
(45, 'hrushikesh', 'shetty', 'm', 'diva', 9, 22-8-13, 25-8-13, 20, 'covid'),
(46, 'abhijeet', 'kumar', 'm', 'thakurli', 12, 24-8-13, 27-8-13, 3, 'rosacea'),
(47, 'shreyas', 'shukla', 'm', 'byculla', 34, 25-8-13, 29-8-13, 5, 'muscular_dystrophy'),
(48, 'deepak', 'mahahan', 'm', 'karjat', 15, 26-8-13, 27-8-13, 1, 'astma'),
(49, 'kapil', 'sharma', 'm', 'ulhasnagar', 22, 27-8-13, 28-8-13, 50, 'thyroid'),
(50, 'shiva', 'kumar', 'm', 'lower parel', 5, 28-8-13, 30-8-13, 7,'typhoid');

create table doctor(
doctor_id int not null,
doctor_name varchar(255) not null,
gender varchar(255) not null,
qualification varchar(255) not null,
job_description varchar(255) not null,
hospital_name varchar(255) not null,
primary key (doctor_id));

alter table doctor add column salary int;

insert into doctor
value(1,'dr.praniti','f', 'md', 'pulmonologist','bhanujyot_hospital',150000),
(2, 'dr.nita', 'f', 'board_certified', 'peditrition', 'sai_hospital',120000),
(3, 'dr.sanjog','m', 'mbbs', 'dermatologist', 'sai_swastik_hospital', 140000),
(4, 'dr.ameya', 'm', 'md', 'opthalmologist', 'shree_hospital', 200000),
(5, 'dr.sanjay', 'm', 'bpt', 'physiotherapist', 'amay_hospital', 100000),
(6, 'dr.priyanka','f', 'bds','dentist', 'khopkar_hospital',80000),
(7, 'dr.tushar','m','mbbs','genral_surgen', 'sai_deep_hospital', 150000),
(8, 'dr.nisha', 'f', 'ms', 'gastroenterologist', 'isha_hospital',120000),
(9, 'dr.roshni', 'f', 'md', 'genral_surgen', 'nivedita_hospital', 130000),
(10, 'dr.jagruti', 'f', 'mbbbs', 'genral_pratictioner', 'kokilaban_hospital', 200000),
(11, 'dr.karishma', 'f', 'md', 'orthopedic', 'jupiter_hospital',180000),
(12, 'dr.niraj', 'm', 'bams', 'ayrveda', 'sanghavi_hospital', 120000),
(13, 'dr.aditya', 'm', 'bpt', 'physiotherapist', 'patil_hospital', 100000),
(14, 'dr,shravani', 'f', 'bhms', 'homeopethic', 'shree_hospital', 120000),
(15, 'dr.pranay', 'm', 'bsms', 'ayurveda', 'shree_hospital', 130000),
(16, 'dr,nandini', 'f', 'bpt', 'physical_therapy', 'om_hospital', 100000),
(17, 'dr.sunanda', 'f', 'bnvs', 'naturopathy_physician', 'sai_hospital', 110000),
(18, 'dr,mrunal', 'f', 'bsms', 'ayurvedic_pratictioner', 'civil_hospital',980000),
(19, 'dr.kalyani', 'f', 'md', 'surgen', 'central_hospital', 190000),
(20, 'dr,shraddha','f', 'mbbs', 'clinical_resurch', 'star_hospital', 180000),
(21, 'dr.tejas', 'm', 'ms', 'surgen', 'metro_hospital', 190000),
(22, 'dr.rohit', 'm', 'bpt', 'therpy_manager', 'shree_hospital', 123000),
(23, 'dr.amita', 'f', 'bds', 'dentist', 'smile_hospital', 900000),
(24, 'dr.amisha', 'f', 'md', 'anesthesiologist', 'maa_hospital', 120000),
(25, 'dr.sushmita', 'f', 'md', 'dermitologist', 'star_multispeciality_hospital', 200000),
(26, 'dr,lavina', 'f', 'bhms', 'homeopathic', 'om_hospital', 100000),
(27, 'dr.jay', 'm', 'mbbs', 'surgen', 'vitthal_krupa_hospital', 159000),
(28, 'dr.swaraj', 'm', 'bams', 'physician', 'shrusti_clinic', 120000),
(29, 'dr.smruti', 'f', 'mbbs', 'surgen', 'shrusti_clinic', 110000),
(30, 'dr.anil', 'm', 'mbbs', 'dermitologist', 'vitthal_krupa_hospital', 180000),
(31, 'dr.swarali', 'f', 'ms', 'physician', 'gurukrupa_clinic', 110000),
(32, 'dr.patel', 'm', 'mbbs', 'surgen', 'vijay_clinic', 120000),
(33, 'dr.savita', 'f', 'bhms', 'homeopathic', 'bhakti_hospital', 130000),
(34, 'dr.sujit', 'm', 'bds', 'dentist', 'sai_krupa_hospital', 100000),
(35, 'dr.yamini', 'f', 'md', 'obstetrics', 'v_hospital', 159000),
(36, 'dr.yadnesh', 'm', 'bams', 'physician', 'saloni_clinic', 120000),
(37, 'dr,lavina', 'f', 'md', 'obstetrics', 'chaitanya_hospital', 190000),
(38, 'dr.sanjay', 'm', 'md', 'orthopedic_surgen', 'krupa_hospital', 167000),
(39, 'dr.yatish', 'm', 'mbbs', 'surgen', 'the_kalyan_hospital', 178000),
(40, 'dr.snehal', 'f', 'bds', 'dentist', 'shruti_clinic', 129000),
(41, 'dr.prachiti', 'f', 'mbbs', 'surgen', 'nisha_clinic', 118000),
(42, 'dr.swati', 'f', 'mbbs', 'dermitologist', 'balaji_hospital', 189000),
(43, 'dr.sumati', 'f', 'ms', 'podiatry', 'jari_mari_clinic', 119000),
(44, 'dr.hasina', 'f', 'mbbs', 'surgen', 'holy_cross', 167000),
(45, 'dr.steve_jorge', 'm', 'md', 'surgen', 'holy_faith_hospital', 189000),
(46, 'dr.ketan', 'm', 'mbbs', 'dermitologist', 'hetal_hospital', 180000),
(47, 'dr.mariyam', 'f', 'ms', 'obstetrics', 'city_hospital', 200000),
(48, 'dr.saira', 'f', 'mbbs', 'surgen', 'kem_hospital', 250000),
(49, 'dr.samayra', 'f', 'mbbs', 'ent_specialist', 'jupiter_hospital',230000),
(50, 'dr.pooja', 'f', 'ms', 'cardiologist', 'fatima_hospital', 250000);

select * from patient;
select * from doctor;
1.select patient_first_name, patient_last_name, gender from patient;

2.select patient_first_name, patient_last_name, gender from patient
where gender= 'f';

3.select patient_id, patient_first_name, patient_last_name from patient limit 30;

4.select avg(salary) from doctor;

5.select doctor_id, salary from doctor where salary >100000;

6.select patient_id, patient_first_name, patient_last_name from patient
where patient_last_name= 'pawar';

7.select* from patient
where patient_id>=10 and patient_id<=30;

8.select * from patient
where address= 'kalyan'or address='thane'or address='nagpur';

9.select * from patient
where patient_first_name like'%a';

10.select * from doctor 
where doctor_name like'%p%';

11.select * from patient 
where patient_first_name = "seeta" 
order by patient_last_name;

12.select * from doctor
where gender = 'f'
order by doctor_name;

13.select patient_first_name, patient_last_name,
concat(patient_first_name," ", patient_last_name),
length(concat(patient_first_name," ", patient_last_name))from patient
order by patient_last_name;

14.select left(patient_first_name,4),
right(patient_last_name,3) from patient;

15.select* from patient where doctor_id=1;

16.select count(doctor_id) from patient where doctor_id=1;

17.select patient_first_name, trim(  patient_first_name   ) from patient;  

18.select patient_first_name, trim( both 'a'from patient_first_name   ) from patient;   

19.select locate('eta',patient_first_name) from patient;

20.select repeat(patient_last_name,3)from patient;

21.select patient.patient_first_name, patient.patient_last_name, doctor.doctor_name
from patient
inner join doctor
on patient.patient_id = doctor.doctor_id;

22.select patient.patient_first_name, patient.patient_last_name, doctor.doctor_name
from patient
right join doctor
on patient.patient_id = doctor.doctor_id;

23.select doctor.doctor_name, doctor.gender, patient.patient_first_name, patient.patient_last_name
from doctor
inner join patient
on doctor.doctor_id = patient.patient_id;

24select patient_id, patient_first_name from patient
union
select doctor_id, doctor_name from doctor; 

25.select patient_id, patient_first_name from patient
union all
select doctor_id, doctor_name from doctor;

26.create view hospital as
select patient_first_name, patient_last_name, gender from patient;
select* from hospital;

27.create view hospitals as
select doctor_id, doctor_name, gender from doctor;
select* from hospitals;

28.select * from patient
where(select patient_id>5);

29.select * from doctor
where(select doctor_id>15);
