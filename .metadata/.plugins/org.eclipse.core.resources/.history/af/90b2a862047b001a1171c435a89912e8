package com.example.domain;

import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;
import javax.persistence.PrePersist;
import javax.persistence.PreUpdate;

import java.util.*;
public class Project {
	@Id
	@GeneratedValue(strategy = GenerationType.IDENTITY)
	private Long id;
	private String projectName;
	private String projectIdentifier;
	public Long getId() {
		return id;
	}
	public Project() {
		super();
		// TODO Auto-generated constructor stub
	}
	public void setId(Long id) {
		this.id = id;
	}
	public String getProjectName() {
		return projectName;
	}
	public Project(Long id, String projectName, String projectIdentifier, String description, Date start_date,
			Date end_date, Date created_at) {
		super();
		this.id = id;
		this.projectName = projectName;
		this.projectIdentifier = projectIdentifier;
		this.description = description;
		this.start_date = start_date;
		this.end_date = end_date;
		this.created_at = created_at;
	}
	public void setProjectName(String projectName) {
		this.projectName = projectName;
	}
	public String getProjectIdentifier() {
		return projectIdentifier;
	}
	public void setProjectIdentifier(String projectIdentifier) {
		this.projectIdentifier = projectIdentifier;
	}
	public String getDescription() {
		return description;
	}
	public void setDescription(String description) {
		this.description = description;
	}
	public Date getStart_date() {
		return start_date;
	}
	public void setStart_date(Date start_date) {
		this.start_date = start_date;
	}
	public Date getEnd_date() {
		return end_date;
	}
	public void setEnd_date(Date end_date) {
		this.end_date = end_date;
	}
	private String description;
	private Date start_date;
	private Date end_date;
	private Date created_at;
	@PrePersist
	public void onCreate()
	{
		
		this.created_at=new Date();
	}
	@PreUpdate
	public void onUpdate()
	{
		this.created_at=new Date();
	}

}
