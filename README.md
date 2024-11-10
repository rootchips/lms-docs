# LMS

### Create User
#### Table - `core_user`
##### Sample data
```json
 {
  "idst": "11840",
  "userid": "\/admin",
  "firstname": "Roslan",
  "lastname": "Saidi",
  "pass": "$2y$10$ztpwqX2hGTyk\/ZWknN6WjuFK1l\/UtcmPEgd\/4gMbt\/kWJccwA.KA2",
  "email": "roslansaidi@ymail.com",
  "level": "0",
  "lastenter": "2024-09-30 15:17:30",
  "valid": "1",
  "force_change": "0",
  "privacy_policy": "0",
  "created_at": "2024-09-30 23:15:57",
  "updated_at": "2024-09-30 23:17:30"
 }
 ```

### Create course
##### Table - `learning_course`
##### Sample data
```json
{
  "idCourse": "2",
  "idCategory": "0",
  "code": "F01",
  "name": "PERKHIDMATAN AWAM",
  "lang_code": "english",
  "status": "2",
  "level_show_user": "0",
  "subscribe_method": "2",
  "linkSponsor": "http:\/\/",
  "mediumTime": "0",
  "permCloseLO": "0",
  "userStatusOp": "8",
  "difficult": "medium",
  "show_progress": "1",
  "show_time": "1",
  "show_who_online": "1",
  "show_extra_info": "0",
  "show_rules": "0",
  "date_begin": "0000-00-00",
  "date_end": "0000-00-00",
  "hour_begin": "-1",
  "hour_end": "-1",
  "valid_time": "0",
  "max_num_subscribe": "0",
  "min_num_subscribe": "0",
  "max_sms_budget": "0",
  "selling": "0",
  "course_type": "elearning",
  "point_to_all": "0",
  "course_edition": "0",
  "create_date": "2024-09-30 15:17:55",
  "used_space": "0",
  "course_vote": "0",
  "allow_overbooking": "0",
  "can_subscribe": "1",
  "direct_play": "0",
  "use_logo_in_courselist": "1",
  "show_result": "0",
  "credits": "0",
  "auto_unsubscribe": "0",
  "id_menucustom": "1",
  "sendCalendar": "0",
  "calendarId": "360f0f0c-013c-4d1b-974b-2ef7bd67a0f9",
  "created_at": "2024-09-30 23:17:55",
  "updated_at": "2024-09-30 23:17:55"
 }
 ```
 
### User Subscribe to course
#### Table - `learning_courseuser`
##### Sample data (level - 3 == student)
```json
{
  "idUser": "11840",
  "idCourse": "2",
  "edition_id": "0",
  "level": "3",
  "date_inscr": "0000-00-00 00:00:00",
  "status": "0",
  "waiting": "0",
  "subscribed_by": "11840",
  "absent": "0",
  "cancelled_by": "0",
  "new_forum_post": "0",
  "requesting_unsubscribe": "0",
  "id": "1",
  "created_at": "2024-09-30 23:17:55",
  "updated_at": "2024-09-30 23:17:55"
 }
 ```
 
### Create FAQ in Course (Content)
#### Table - learning_faq_cat
##### Sample data
```json
 {
  "idCategory": "1",
  "title": "TestFAQ",
  "description": "Testing FAQ",
  "author": "11840",
  "created_at": "2024-09-30 23:56:59",
  "updated_at": "2024-09-30 23:56:59"
 }
 ```
 
### Create Glossary in Course (Content)
#### Table - `learning_glossary`
##### Sample data
```json
 {
  "idGlossary": "1",
  "title": "Glossary Test",
  "description": "Glossary",
  "author": "11840",
  "created_at": "2024-09-30 23:59:19",
  "updated_at": "2024-09-30 23:59:19"
 }
 ```
 
### Create HTML Page (with File) in Course
#### Table - `learning_htmlpage`
#### Sample data
```json
{
  "idPage": "1",
  "title": "HTML Test",
  "textof": "Test",
  "author": "11840",
  "created_at": "2024-10-01 00:02:05",
  "updated_at": "2024-10-01 00:02:05"
 }
 ```
#### Table - `learning_htmlpage_attachment`
#### Location file and sample data
```sh
ls -alF root-project/files/appLms/htmlpages/
```
```json
 {
  "id": "1",
  "idpage": "1",
  "file": "2_75_1727712125_N3C System Generated Receipt.pdf",
  "title": "Generated Receipt.pdf",
  "created_at": "2024-10-01 00:02:05",
  "updated_at": "2024-10-01 00:02:05"
 }
```

### Content
### All content from above will create data in this table too
#### Table - `learning_organization`
##### Sample data
 ```json
[
 {
  "idOrg": "1",
  "idParent": "0",
  "path": "\/root\/00000001",
  "lev": "1",
  "title": "Directory 1",
  "idResource": "0",
  "idCategory": "0",
  "idUser": "0",
  "idAuthor": "0",
  "dateInsert": "0000-00-00 00:00:00",
  "idCourse": "2",
  "isTerminator": "0",
  "idParam": "0",
  "visible": "1",
  "milestone": "-",
  "width": "0",
  "height": "0",
  "publish_for": "0",
  "ignoreScore": "0",
  "created_at": "2024-09-30 23:52:11",
  "updated_at": "2024-09-30 23:52:11"
 },
 {
  "idOrg": "2",
  "idParent": "0",
  "path": "\/root\/00000002",
  "lev": "1",
  "title": "TestFAQ",
  "objectType": "faq",
  "idResource": "1",
  "idCategory": "0",
  "idUser": "0",
  "idAuthor": "11840",
  "version": "1.0",
  "dateInsert": "2024-09-30 15:56:59",
  "idCourse": "2",
  "isTerminator": "0",
  "idParam": "1",
  "visible": "1",
  "width": "0",
  "height": "0",
  "publish_for": "0",
  "ignoreScore": "0",
  "created_at": "2024-09-30 23:56:59",
  "updated_at": "2024-09-30 23:56:59"
 },
 {
  "idOrg": "3",
  "idParent": "0",
  "path": "\/root\/00000003",
  "lev": "1",
  "title": "Glossary Test",
  "objectType": "glossary",
  "idResource": "1",
  "idCategory": "0",
  "idUser": "0",
  "idAuthor": "11840",
  "version": "1.0",
  "dateInsert": "2024-09-30 15:59:19",
  "idCourse": "2",
  "isTerminator": "0",
  "idParam": "3",
  "visible": "1",
  "width": "0",
  "height": "0",
  "publish_for": "0",
  "ignoreScore": "0",
  "created_at": "2024-09-30 23:59:19",
  "updated_at": "2024-09-30 23:59:19"
 },
 {
  "idOrg": "4",
  "idParent": "0",
  "path": "\/root\/00000004",
  "lev": "1",
  "title": "HTML Test",
  "objectType": "htmlpage",
  "idResource": "1",
  "idCategory": "0",
  "idUser": "0",
  "idAuthor": "11840",
  "version": "1.0",
  "dateInsert": "2024-09-30 16:02:05",
  "idCourse": "2",
  "isTerminator": "0",
  "idParam": "5",
  "visible": "1",
  "width": "0",
  "height": "0",
  "publish_for": "0",
  "ignoreScore": "0",
  "created_at": "2024-10-01 00:02:05",
  "updated_at": "2024-10-01 00:02:05"
 },
 {
  "idOrg": "5",
  "idParent": "0",
  "path": "\/root\/00000005",
  "lev": "1",
  "title": "Screenshot 2024-09-30 at 11.55.49 PM.png",
  "objectType": "item",
  "idResource": "1",
  "idCategory": "0",
  "idUser": "0",
  "idAuthor": "11840",
  "version": "1.0",
  "dateInsert": "2024-09-30 16:08:29",
  "idCourse": "2",
  "isTerminator": "0",
  "idParam": "7",
  "visible": "1",
  "width": "0",
  "height": "0",
  "publish_for": "0",
  "ignoreScore": "0",
  "created_at": "2024-10-01 00:08:29",
  "updated_at": "2024-10-01 00:08:29"
 }
]
 ```

### Test
#### To create a test and put it same as learning_organization
#### Table - `learning_test`
##### Sample Data
```
  {
    "idTest": 9,
    "author": 11840,
    "title": "TEST",
    "description": "TEST",
    "point_type": 0,
    "point_required": 0,
    "display_type": 0,
    "order_type": 0,
    "shuffle_answer": 0,
    "question_random_number": 0,
    "save_keep": 0,
    "mod_doanswer": 1,
    "can_travel": 1,
    "show_only_status": 0,
    "show_score": 1,
    "show_score_cat": 0,
    "show_doanswer": 0,
    "show_solution": 0,
    "time_dependent": 0,
    "time_assigned": 0,
    "penality_test": 0,
    "penality_time_test": 0,
    "penality_quest": 0,
    "penality_time_quest": 0,
    "max_attempt": 0,
    "hide_info": 0,
    "order_info": "",
    "cf_info": "",
    "use_suspension": 0,
    "suspension_num_attempts": 0,
    "suspension_num_hours": 0,
    "suspension_prerequisites": 0,
    "chart_options": "",
    "mandatory_answer": 0,
    "score_max": 0,
    "obj_type": "test",
    "retain_answers_history": 0,
    "gradimento": null,
    "created_at": "2024-11-10 23:39:50",
    "updated_at": "2024-11-10 23:39:50"
  }
```

### Test
#### To create a question in a test
##### Table - `learning_testquest`
###### Sample Data
```
  {
    "idQuest": 9,
    "idTest": 9,
    "idCategory": 0,
    "type_quest": "choice",
    "title_quest": "What is 1+1?",
    "difficult": 3,
    "time_assigned": 0,
    "sequence": 1,
    "page": 1,
    "shuffle": 0,
    "created_at": "2024-11-10 23:46:51",
    "updated_at": "2024-11-10 23:46:51"
  }
```

### Test
#### To create multiple answer in a question
#### Table - `learning_testquestanswer`
##### Sample Data
```
[
  {
    "idAnswer": 17,
    "idQuest": 9,
    "sequence": 0,
    "is_correct": 0,
    "answer": "1",
    "comment": "",
    "score_correct": 100,
    "score_incorrect": 10,
    "created_at": "2024-11-10 23:46:51",
    "updated_at": "2024-11-10 23:46:51"
  },
  {
    "idAnswer": 18,
    "idQuest": 9,
    "sequence": 0,
    "is_correct": 1,
    "answer": "2",
    "comment": "",
    "score_correct": 100,
    "score_incorrect": 10,
    "created_at": "2024-11-10 23:46:51",
    "updated_at": "2024-11-10 23:46:51"
  },
  {
    "idAnswer": 19,
    "idQuest": 9,
    "sequence": 0,
    "is_correct": 0,
    "answer": "3",
    "comment": "",
    "score_correct": 100,
    "score_incorrect": 10,
    "created_at": "2024-11-10 23:46:51",
    "updated_at": "2024-11-10 23:46:51"
  }
]
```

### Test
#### To attempt answer a question
#### Table - `learning_testtrack`
##### Sample Data
```
  {
    "idTrack": 9,
    "idUser": 11840,
    "idReference": 25,
    "idTest": 9,
    "date_attempt": "2024-11-10 23:49:31",
    "date_attempt_mod": null,
    "date_end_attempt": "2024-11-10 23:51:24",
    "last_page_seen": 1,
    "last_page_saved": 0,
    "number_of_save": 1,
    "number_of_attempt": 1,
    "score": 100,
    "bonus_score": 0,
    "score_status": "valid",
    "comment": "",
    "attempts_for_suspension": 0,
    "suspended_until": null,
    "created_at": "2024-11-10 23:49:26",
    "updated_at": "2024-11-10 23:51:24"
  }
```
### Test
#### To submit answer a question
#### Table - `learning_testtrack_answer`
##### Sample Data
```
[
  {
    "idTrack": 9,
    "idQuest": 9,
    "idAnswer": 17,
    "score_assigned": 100,
    "more_info": "",
    "manual_assigned": 0,
    "user_answer": 0,
    "number_time": 1,
    "id": 21,
    "created_at": "2024-11-10 23:51:24",
    "updated_at": "2024-11-10 23:51:24"
  },
  {
    "idTrack": 9,
    "idQuest": 9,
    "idAnswer": 18,
    "score_assigned": 100,
    "more_info": "",
    "manual_assigned": 0,
    "user_answer": 1,
    "number_time": 1,
    "id": 22,
    "created_at": "2024-11-10 23:51:24",
    "updated_at": "2024-11-10 23:51:24"
  },
  {
    "idTrack": 9,
    "idQuest": 9,
    "idAnswer": 19,
    "score_assigned": 100,
    "more_info": "",
    "manual_assigned": 0,
    "user_answer": 0,
    "number_time": 1,
    "id": 23,
    "created_at": "2024-11-10 23:51:24",
    "updated_at": "2024-11-10 23:51:24"
  }
]
```

### Test
#### To track test track page
#### Table - `learning_testtrack_page`
##### Sample Data
```
  {
    "idTrack": 9,
    "page": 1,
    "display_from": "2024-11-10 23:49:31",
    "display_to": "2024-11-10 23:51:24",
    "accumulated": 0,
    "id": 10,
    "created_at": "2024-11-10 23:49:31",
    "updated_at": "2024-11-10 23:51:24"
  }
```

### Test
#### To record question track page
#### Table - `learning_testtrack_quest`
##### Sample Data
```
  {
    "idTrack": 9,
    "idQuest": 9,
    "page": 1,
    "id": 10,
    "created_at": "2024-11-10 23:49:31",
    "updated_at": "2024-11-10 23:49:31"
  }
```

### Test
#### To record how much attempt / timing user answer a question
#### Table - `learning_testtrack_times`
##### Sample Data
```
  {
    "idTrack": 9,
    "idReference": 25,
    "idTest": 9,
    "date_attempt": "2024-11-10 23:51:24",
    "number_time": 1,
    "score": 100,
    "score_status": "valid",
    "date_begin": "2024-11-10 23:49:31",
    "date_end": "2024-11-10 23:51:24",
    "time": 113,
    "id": 10,
    "created_at": "2024-11-10 23:51:24",
    "updated_at": "2024-11-10 23:51:24"
  }
```
