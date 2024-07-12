pipeline {
	agent any

	stages {
		stage('Checkout') {
			steps {
				echo "This is git clone stage"
				sh "sleep 5"
				sh "ls -lrt"
			}
		}

		stage('Build') {
			steps {
				sh ''' 
					echo Complie and build the package
				    sleep 5
				'''
			}
		}

		stage('Test') {
			steps {
				sh """
					#!/bin/bash
					echo This is Integration testing
					sleep 5
					ls -lrt
				"""
			}
		}
	}
}
