# Ruby on Rails Tutorial: Sample App

[![Build Status](https://travis-ci.org/cunctat0r/nanoblog3.svg?branch=master)](https://travis-ci.org/cunctat0r/nanoblog3)
[![Code Climate](https://codeclimate.com/github/cunctat0r/nanoblog3/badges/gpa.svg)](https://codeclimate.com/github/cunctat0r/nanoblog3)
[![Test Coverage](https://codeclimate.com/github/cunctat0r/nanoblog3/badges/coverage.svg)](https://codeclimate.com/github/cunctat0r/nanoblog3/coverage)
[![Issue Count](https://codeclimate.com/github/cunctat0r/nanoblog3/badges/issue_count.svg)](https://codeclimate.com/github/cunctat0r/nanoblog3)
[![security](https://hakiri.io/github/cunctat0r/nanoblog3/master.svg)](https://hakiri.io/github/cunctat0r/nanoblog3/master)

This is the sample application for the
[*Ruby on Rails Tutorial*](http://www.railstutorial.org/)
by [Michael Hartl](http://www.michaelhartl.com/).

To use successfully Amazon AWS S3 buckets, you need set up access policies and CORS configuration.  Default CORS configuration works for me,  and for access policy I use the following: 

```
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Sid": "",
			"Effect": "Allow",
			"Principal": "*",
			"Action": "s3:*",
			"Resource": [
				"arn:aws:s3:::my-bucket",
				"arn:aws:s3:::my-bucket/*"
			]
		}
	]
}
```