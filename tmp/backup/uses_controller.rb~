class UsesController < ApplicationController
  # GET /uses
  # GET /uses.json
  def index
    @uses = Use.all

    respond_to do |format|
      format.html # index.html.erb
      format.json { render json: @uses }
    end
  end

  # GET /uses/1
  # GET /uses/1.json
  def show
    @use = Use.find(params[:id])

    respond_to do |format|
      format.html # show.html.erb
      format.json { render json: @use }
    end
  end

  # GET /uses/new
  # GET /uses/new.json
  def new
    @use = Use.new

    respond_to do |format|
      format.html # new.html.erb
      format.json { render json: @use }
    end
  end

  # GET /uses/1/edit
  def edit
    @use = Use.find(params[:id])
  end

  # POST /uses
  # POST /uses.json
  def create
    @use = Use.new(params[:use])

    respond_to do |format|
      if @use.save
        format.html { redirect_to @use, notice: 'Use was successfully created.' }
        format.json { render json: @use, status: :created, location: @use }
      else
        format.html { render action: "new" }
        format.json { render json: @use.errors, status: :unprocessable_entity }
      end
    end
  end

  # PUT /uses/1
  # PUT /uses/1.json
  def update
    @use = Use.find(params[:id])

    respond_to do |format|
      if @use.update_attributes(params[:use])
        format.html { redirect_to @use, notice: 'Use was successfully updated.' }
        format.json { head :no_content }
      else
        format.html { render action: "edit" }
        format.json { render json: @use.errors, status: :unprocessable_entity }
      end
    end
  end

  # DELETE /uses/1
  # DELETE /uses/1.json
  def destroy
    @use = Use.find(params[:id])
    @use.destroy

    respond_to do |format|
      format.html { redirect_to uses_url }
      format.json { head :no_content }
    end
  end
end
