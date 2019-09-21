# Yuliya Khvan

##### Address: Almaty, Djandarbekova, 169-9 || E-mail: yuliyahvan@yahoo.com || Mobile: +7 701 789-20-43

![Image](./assets/images/my_image.jpg)

### Summary
Become a full-stack developer (front-end & back-end) using life & work experience (9 years experience in finance, audit); 
Thirsty for continuous growth & development, getting new knowledge; self- challenged person (change in work experience, industry, profession); 

Good analytical skills, goal-oriented, self-managed, active, responsible, hard-working, positive thinking, open for newness, mobile, disciplined, professional ethics supporter, healthy lifestyle supporter, sport active (marathoner, hiker)

### Skills
* Programming language: Python
* Frameworks: Django
* Version control: Git
* CI / CD: TravisCI, Gunicorn, Ngnix, AWS / DO, Docker, Docker-compose
* TDD: Pytest, Pep8, Flake8

### Code examples
```python
from django.db import models
from django.contrib.auth.models import User


class Profile(models.Model):
    user = models.OneToOneField(User, on_delete=models.CASCADE)
    birthday = models.DateField(null=True, blank=True)
    contact_number = models.CharField(max_length=20, null=True)
```
```python
def test_register_view(db, client, data):
    response = client.get('/register/')
    assert response.status_code == 200

    response = client.post(
        '/register/', {'username': 'test', 'password': 'test'}
    )
    assert response.status_code == 200
```
```python
from django.contrib import admin
from django.contrib.auth.admin import UserAdmin as BaseUserAdmin
from django.contrib.auth.models import User
from .models import Image, Profile


class ProfileInline(admin.StackedInline):
    model = Profile
    can_delete = False
    verbose_name_plural = 'profile'


class UserAdmin(BaseUserAdmin):
    inlines = (ProfileInline, )


admin.site.register(Image)
admin.site.unregister(User)
admin.site.register(User, UserAdmin)
```

### Experience
#### *Projects:*
* Django project for internet shop on github link: https://github.com/xx3u/django_module
* Social network project (in process) on domain: http://xx3u.ml/ and on github link: https://github.com/xx3u/social_network

#### *Intern in iMoney LLP*
*2019 August - present*   
iMoney - strategy developement in decision-making in credit process, terminals for micro-credit organizations [3min.kz](https://3min.kz/)
- Docker, docker-compose; 
- Sql db on postgres container; 
- Celery tasks & logs;
- New credit scoring system code;

#### *Head of Controlling, Central Asia in Sanofi-Aventis, Kazakhstan LLP*
*2018 June - 2019 July*
- Team management of 5 people, consolidation over cluster including 8 countries (Kazakhstan, Uzbekistan, Georgia, Armenia, Azerbaijan, Turkmenistan, Kyrgyzstan, Tajikistan);
- Budget Cycles, Reporting, Transfer Pricing, Internal Control;

#### *Finance Controller in Sanofi-Aventis, Kazakhstan LLP*
*2016 August - 2018 May*
- Consolidation over Central Asia cluster, Budgeting, Reporting;

#### *Finance Controlling Supervisor in Abdi Ibrahim Global Pharm LLP*
*2014 July - 2016 July*
- Overall responsibility for budgeting & reporting processes, reporting to & communication with HO;
- Preparation of analytical information for Board of Directors and Business Review meetings, year-end forecasting/Business Plan;

#### *Financial Analyst in Abdi Ibrahim Global Pharm LLP*
*2013 July - 2014 June*
- Preparation of budget, financial reporting package

#### *Experienced Consultant in PricewaterhouseCoopers LLP*
*2010 September - 2013 June*
- Experience in auditing of companies from oil&gas, retail industry, manufacturing and logistics businesses;
- Specialization in accounting and audit, the risk assessment and review of internal controls;
- Audit of financial statements prepared in compliance with PSA/JOA/IFRS of operating company;
- Audit of retail & consumer multinational company with relevant assessment of internal control system;

### Education
- 2019: Codecademy: Introduction to Html; Learn CSS
- 2019: RS School: JavaScript Development Online
- 2019: Vault77 school: Django
- 2018: Vault77 school: Python
- 2010: KIMEP: MBA, Major in Accounting (Almaty)
- 2008: UWED: Bachelor in International Economic Relations (Tashkent)


### English
EPAM English test results: B1

Usage on every work starting from PwC in audit, all work documentation was on english as well as communication with Partners and Clients. 

During work in Abdi Ibrahim Global Pharm, english used extensively (in communication) as my direct manager was from Turkey and all correspondance with HO was on english.

During work in Sanofi all correspondance, reporting (including presentations, deck and packages) and communication with HQ (located in France mainly) was on english. 
